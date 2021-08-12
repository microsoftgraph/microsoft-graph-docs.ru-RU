---
author: daspek
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
description: Ресурс columnLink для объекта contentType связывает ресурс columnDefinition сайта с соответствующим типом контента.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c14edb1baf1b586e193f26df60f74d6d9b846aeae3f0eb2a4d6eb2422581313a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124523"
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
| **id**        | строка | Уникальный идентификатор столбца.
| **name**      | строка | Имя столбца в этом типе контента.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/ColumnLink"
} -->

