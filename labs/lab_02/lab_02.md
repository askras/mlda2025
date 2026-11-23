---
jupyter:
  jupytext:
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.19.5
  kernelspec:
    display_name: Python 3
    language: python
    name: python3
---

```python
import matplotlib.pyplot as plt
import numpy as np

from matplotlib.patches import Circle

mu = 1
sigma = 1
dots_x = np.random.normal(mu, sigma, 100)
dots_y = np.random.normal(mu, sigma, 100)

fig, axes = plt.subplots(figsize=(8, 8))
axes.set_aspect("equal")
axes.scatter(dots_x, dots_y, label="Норм. распр. точки")
axes.scatter(mu, mu, color="black", label="μ")

distances = np.sqrt((dots_x - mu) ** 2 + (dots_y - mu) ** 2)

circle_99 = Circle(
    (mu, mu), np.percentile(distances, 99), color="red", fill=False, linewidth=2,
    label="99% точек"
)

circle_3sigma = Circle(
    (mu, mu), 3 * sigma, color="black", fill=False, linewidth=2, label="3σ радиус"
)

axes.add_patch(circle_99)
axes.add_patch(circle_3sigma)
axes.legend()
```

## Задание 2 

Используйте вспомогательный график, чтобы нарисовать гистограммы с 10 сегментами для каждого измерения и построить график плотности вдоль гистограммы для данных из первого задания.

```python executionInfo={"elapsed": 316, "status": "ok", "timestamp": 1694439806964, "user": {"displayName": "Sergey Korpachev", "userId": "09181340988160569540"}, "user_tz": -180} id="8f1ca529"
fig, axes = plt.subplots(1, 2, figsize=(14, 5))

x = np.linspace(mu - 4 * sigma, mu + 4 * sigma, 300)

density = (
    1 / (sigma * np.sqrt(2 * np.pi)) * np.exp(-((x - mu) ** 2) / (2 * sigma ** 2))
)

axes[0].hist(
    dots_x,
    bins=10,
    density=True,
    edgecolor="black",
    label="Гистограмма"
)

axes[0].plot(
    x,
    density,
    linewidth=2,
    label="Плотность"
)

axes[0].set_title("Распределение X")
axes[0].set_xlabel("X")
axes[0].set_ylabel("Плотность")
axes[0].legend()
axes[0].grid(alpha=0.3)

axes[1].hist(
    dots_y,
    bins=10,
    density=False,
    edgecolor="black",
    label="Гистограмма"
)

axes[1].plot(
    x,
    density,
    linewidth=2,
    label="Плотность"
)

axes[1].set_title("Распределение Y")
axes[1].set_xlabel("Y")
axes[1].set_ylabel("Плотность")
axes[1].legend()
axes[1].grid(alpha=0.3)

plt.tight_layout()
plt.show()

```

<!-- #region id="6e8398b0" -->

### Задание  3 

Загрузите набор данных ["Ирисы Фишера"](https://ru.wikipedia.org/wiki/Ирисы_Фишера). 
Создайте тепловую карту с корреляциями между признаками объектов, строки и столбцы которой должны быть подписаны названиями признаков. 
Важно использовать matplotlib. 
Прямая корреляция должна отображаться зеленым цветом, обратная &mdash; красным, а отсутствие корреляции &mdash; белым. 
Сделайте график достаточно крупным.

**Подсказка:** используйте `plt.xticks`, `plt.yticks`, `plt.imshow`, `plt.colorbar`


<!-- #endregion -->

```python id="b6414734"
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from matplotlib.colors import LinearSegmentedColormap

df = pd.read_csv('iris.csv')

print(df.head())

feature_cols = ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']
features = df[feature_cols]


corr_matrix = np.corrcoef(features.T)  # форма (4, 4)

cmap = LinearSegmentedColormap.from_list('my_cmap', ['green', 'white', 'red'])

fig, ax = plt.subplots(figsize=(8, 6))

im = ax.imshow(corr_matrix, cmap=cmap, vmin=-1, vmax=1)


ax.set_xticks(np.arange(len(feature_cols)))
ax.set_yticks(np.arange(len(feature_cols)))
ax.set_xticklabels(feature_cols, rotation=45, ha='right')
ax.set_yticklabels(feature_cols)
ax.set_title('Корреляции между признаками ириса')

for i in range(corr_matrix.shape[0]):
    for j in range(corr_matrix.shape[1]):
        ax.text(j, i, round(corr_matrix[i, j], 2),
                ha='center', va='center', color='black')

fig.colorbar(im, ax=ax)
plt.tight_layout()
plt.show()
```

## Задание 4

Cоздайте такую же тепловую карту, используя `seaborn.heatmap`

```python executionInfo={"elapsed": 293, "status": "ok", "timestamp": 1694439821851, "user": {"displayName": "Sergey Korpachev", "userId": "09181340988160569540"}, "user_tz": -180} id="47f49efd"
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

df = pd.read_csv('iris.csv')

feature_cols = ['sepal_length', 'sepal_width', 'petal_length', 'petal_width']
features = df[feature_cols]

corr_matrix = features.corr() 
print(corr_matrix)


plt.figure(figsize=(8, 6))
sns.heatmap(corr_matrix,
            annot=True,        
            fmt='.2f',         
            cmap='RdYlGn',     
            vmin=-1, vmax=1,   
            square=True,
            linewidths=0.5)

plt.title('Корреляции между признаками ириса (pandas.corr + seaborn)')
plt.tight_layout()
plt.show()
```
