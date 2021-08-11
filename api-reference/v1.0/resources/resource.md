---
title: Тип ресурса OneNoteResource
description: 'Изображение или другой ресурс файла на OneNote странице. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 39945f3086c8470dcbccc9d11a242d71df2a99dfd99977f147b2fcd180d69d24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218417"
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

## <a name="relationships"></a>Связи
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

