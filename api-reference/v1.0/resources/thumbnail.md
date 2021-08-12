---
author: JeremyKelley
ms.date: 09/10/2017
title: Эскиз
localization_priority: Normal
description: Тип ресурса thumbnail представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 66656ed7a286290691182b79cce079110fb602c1157a9eb064ac92c88c5b1cec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163644"
---
# <a name="thumbnail-resource-type"></a>Тип ресурса thumbnail

Пространство имен: microsoft.graph

Тип ресурса **thumbnail** представляет эскиз изображения, видео, документа или любого другого элемента, представленного как растровое изображение.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса **thumbnail** в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание
| :----------- | :----- | :----------------------------------------------------
| height       | Int32  | Высота эскиза в пикселях.
| sourceItemId | String | Уникальный идентификатор элемента, предоставившего эскиз. Доступен только при запросе эскиза папки.
| url          | String | URL-адрес, используемый для получения содержимого эскиза.
| width        | Int32  | Ширина эскиза в пикселях.
| содержимое      | Поток | Поток содержимого для эскиза.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->

