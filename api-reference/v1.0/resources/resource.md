---
title: Тип ресурса oneNoteResource
description: 'Изображение или другой файл ресурса на OneNote страницы. '
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: e304bdcee171350ade75b6253d12e3abfac77856
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034889"
---
# <a name="onenoteresource-resource-type"></a>Тип ресурса oneNoteResource

Пространство имен: microsoft.graph

Изображение или другой файл ресурса на OneNote страницы.

Вы можете получить двоичные данные ресурса, но получение представления объекта ресурса или коллекции ресурсов в формате JSON не поддерживается.

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

URI ресурса файла возвращается при получение HTML-содержимого страницы с помощью следующего запроса:

```
GET ../onenote/pages/{id}/content
```

В HTML-коде `img` `data-fullres-src` страницы тег включает конечные точки для исходного ресурса изображения в атрибуте и оптимизированный образ в атрибуте `src` :
```
<img
    src="image-resource-url"
    data-src-type="media-type"
    data-fullres-src="image-resource-url"
    data-fullres-src-type="media-type" ... />
```

Тег `object` (который представляет такие файлы, как PDF, DOCX и PNG) содержит конечную точку для файлового ресурса в атрибуте `data` :

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type"
    type="media-type" ... />
```

## <a name="properties"></a>Свойства

| Свойство             | Тип            | Описание
|:---------------------|:----------------|:---------------------------------
| содержимое              | Поток          | Поток содержимого
| contentUrl           | Строка (URL-адрес)    | URL-адрес для скачивания содержимого

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение двоичных данных ресурсов](../api/resource-get.md) | Stream |Получение двоичных данных ресурса файла или изображения.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

