---
title: Тип ресурса OneNoteResource
description: 'Изображение или другой ресурс файла на OneNote странице. '
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f0f290329135f828ac36d5e5d805c515f2d9a207
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055852"
---
# <a name="onenoteresource-resource-type"></a>Тип ресурса OneNoteResource

Пространство имен: microsoft.graph

Изображение или другой ресурс файла на OneNote странице.

Вы можете получить двоичные данные ресурса, но получение представления JSON объекта ресурса или коллекции ресурсов не поддерживается.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

Получите двоичные данные определенного ресурса, отправив запрос GET в конечную точку `content` ресурса:

```
GET ../onenote/resources/{id}/content
```

URI ресурса файла возвращается после получения HTML-контента страницы с помощью следующего запроса:

```
GET ../onenote/pages/{id}/content
```

На странице HTML тег содержит конечные точки исходного ресурса изображения в атрибуте и оптимизированный образ `img` `data-fullres-src` в `src` атрибуте:
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

Тег (который представляет файлы, такие как PDF, DOCX и PNG), включает конечную точку для файловой ресурс `object` в `data` атрибуте:

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a>Свойства

| Свойство             | Тип            | Описание
|:---------------------|:----------------|:---------------------------------
| содержимое              | Поток          | Поток контента
| contentUrl           | String (URL)    | URL-адрес для скачивания контента

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получить двоичные данные ресурсов](../api/resource-get.md) | Stream |Извлечение двоичных данных файла или ресурса изображений.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

