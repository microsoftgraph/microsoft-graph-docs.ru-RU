---
title: Тип ресурса Оненотересаурце
description: 'Изображение или другой файловый ресурс на странице OneNote. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: fc4f3962e5be1eeb69598548067b61aa86c9c246
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806299"
---
# <a name="onenoteresource-resource-type"></a>Тип ресурса Оненотересаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изображение или другой файловый ресурс на странице OneNote.

Вы можете получить двоичные данные ресурса, но получение представления объекта ресурса или коллекции ресурсов в формате JSON не поддерживается.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": "String (Stream)",
  "contentUrl": "String"
}

```
Получение двоичных данных определенного ресурса путем отправки запроса GET в `content` конечную точку ресурса:

```
GET ../onenote/resources/{id}/content
```

URI ресурса файла возвращается при получении HTML-контента страницы с помощью следующего запроса:

```
GET ../onenote/pages/{id}/content
```

В HTML-коде страницы `img` тег включает конечные точки для исходного ресурса изображения в `data-fullres-src` атрибуте и оптимизированное изображение в `src` атрибуте:
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

`object`Тег, представляющий файлы, такие как PDF, docx и PNG, включает конечную точку для ресурса файла в `data` атрибуте:

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| content | Модель EDM. Stream||
| contentUrl | String ||

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение двоичных данных ресурса](../api/resource-get.md) | Stream |Получение двоичных данных ресурса файла или изображения.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
