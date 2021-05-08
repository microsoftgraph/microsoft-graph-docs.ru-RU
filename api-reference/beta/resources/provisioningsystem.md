---
title: тип ресурсов provisioningSystem
description: Представляет систему, в которую пользователь был предварительно или из нее.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 2dcc52e4b847648477313d61c8b69b168a8807b1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232983"
---
# <a name="provisioningsystem-resource-type"></a>тип ресурсов provisioningSystem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет систему, в которую пользователь был предварительно или из нее. Например, при предоставлении пользователю Azure Active Directory (Azure AD) в ServiceNow, источником системы является Azure AD, а целевой системой является ServiceNow.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|подробности|[detailsInfo](detailsinfo.md)|Сведения о системе.|
|displayName|String|Имя системы, в которую пользователь был предварительно или из нее.|
|id|String|Идентификатор системы, в которую пользователь был предварительно или из нее.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystem",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


