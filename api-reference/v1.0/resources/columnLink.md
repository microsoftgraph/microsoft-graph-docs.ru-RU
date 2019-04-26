---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: columnLink
localization_priority: Normal
ms.openlocfilehash: 435696cc596f73830104ea8ec0619bf40a462d62
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565788"
---
# <a name="columnlink-resource-type"></a>Тип ресурса ColumnLink

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **columnLink** для объекта [contentType][] связывает ресурс **columnDefinition** сайта с соответствующим типом контента.

[contentType]: contenttype.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **columnLink** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | Уникальный идентификатор столбца.
| **name**      | string | Имя столбца в этом типе контента.

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
