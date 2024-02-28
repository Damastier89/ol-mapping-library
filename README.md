# Ol-Mapping-Library

`ol-mapping-library` это высокопроизводительная многофункциональная библиотека для создания интерактивных карт в Интернете. Она может отображать фрагменты карты, векторные данные и маркеры, загруженные из любого источника, на любой веб-странице. `ol-custom-library` был разработан для дальнейшего использования географической информации всех видов.

## Установка

```
npm i ol-mapping-library
```

```js
import { Map, View } from 'ol-mapping-library'
import TileLayer from 'ol-mapping-library/layer/Tile'
import XYZ from 'ol-mapping-library/source/XYZ'

new Map({
	target: 'map',
	layers: [
		new TileLayer({
			source: new XYZ({
				url: 'https://tile.openstreetmap.org/{z}/{x}/{y}.png',
			}),
		}),
	],
	view: new View({
		center: [0, 0],
		zoom: 2,
	}),
})
```

```css
@import 'ol-mapping-library/ol.css';
```
