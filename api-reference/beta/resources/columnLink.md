---
author: daspek
description: Ресурс columnLink для объекта contentType связывает ресурс columnDefinition сайта с соответствующим типом контента.
ms.date: 09/12/2017
title: columnLink
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ae75a605f8476b9ec25d5aab5cf50f1bf9508c95
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723530"
---
# <a name="columnlink-resource-type"></a>Тип ресурса ColumnLink

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.

[contentType]: contenttype.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **columnLink** в формате JSON.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name&quot;: &quot;string"
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип   | Описание                                   |
| :------- | :----- | :-------------------------------------------- |
| **id**   | строка | Уникальный идентификатор столбца.         |
| **name** | строка | Имя столбца в этом типе контента. |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": []
}
-->
