---
author: daspek
ms.date: 09/12/2017
title: columnLink
ms.localizationpriority: medium
description: Ресурс columnLink для объекта contentType связывает ресурс columnDefinition сайта с соответствующим типом контента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1ad2a7397c18ad8be17a5e5bb27c25ecc84dffa6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113723"
---
# <a name="columnlink-resource-type"></a>Тип ресурса ColumnLink

Пространство имен: microsoft.graph

Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.

[contentType]: contenttype.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **columnLink** в формате JSON.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name&quot;: &quot;string"
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | Уникальный идентификатор столбца.
| **name**      | string | Имя столбца в этом типе контента.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/ColumnLink"
} -->

