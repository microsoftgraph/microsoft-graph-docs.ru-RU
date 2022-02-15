---
title: тип ресурса onenoteResource
description: 'Изображение или другой ресурс файла на OneNote странице. '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: f7a479ec529cae209fef085da2978c3e412a844f
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804922"
---
# <a name="onenoteresource-resource-type"></a>тип ресурса onenoteResource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изображение или другой ресурс файла на OneNote странице.

Вы можете получить двоичные данные ресурса, но получение представления JSON объекта ресурса или коллекции ресурсов не поддерживается.

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

Получите двоичные данные определенного ресурса, отправив запрос GET в конечную `content` точку ресурса:

```http
GET ../onenote/resources/{id}/content
```

URI ресурса файла возвращается после получения HTML-контента страницы с помощью следующего запроса:

```http
GET ../onenote/pages/{id}/content
```

На странице HTML тег `img` `data-fullres-src` содержит конечные точки исходного ресурса изображения в атрибуте и оптимизированный образ в атрибуте `src` :

```html
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

Тег `object` (который представляет файлы, такие как PDF, DOCX и PNG), включает конечную точку для файловой ресурс в атрибуте `data` :

```html
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получить двоичные данные ресурсов](../api/resource-get.md) | Stream |Извлечение двоичных данных файла или ресурса изображений.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| content | Edm.Stream||
| contentUrl | String ||

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


