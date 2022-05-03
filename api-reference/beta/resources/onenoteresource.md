---
title: Тип ресурса onenoteResource
description: 'Изображение или другой файл ресурса на OneNote страницы. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: notes
author: jewan-microsoft
ms.openlocfilehash: 21d0be436241b518e87b0eb36956886808211a0d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176713"
---
# <a name="onenoteresource-resource-type"></a>Тип ресурса onenoteResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изображение или другой файл ресурса на OneNote страницы.

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

Получите двоичные данные определенного ресурса, отправив запрос GET в конечную точку `content` ресурса:

```http
GET ../onenote/resources/{id}/content
```

URI ресурса файла возвращается при получение HTML-содержимого страницы с помощью следующего запроса:

```http
GET ../onenote/pages/{id}/content
```

В HTML-коде `img` `data-fullres-src` страницы тег включает конечные точки для исходного ресурса изображения в атрибуте и оптимизированный образ в атрибуте `src` :

```html
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

Тег `object` (который представляет такие файлы, как PDF, DOCX и PNG) содержит конечную точку для файлового ресурса в атрибуте `data` :

```html
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение двоичных данных ресурсов](../api/resource-get.md) | Stream |Получение двоичных данных ресурса файла или изображения.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| content | Edm.Stream||
| contentUrl | Строка ||

## <a name="relationships"></a>Связи
Отсутствуют.

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


