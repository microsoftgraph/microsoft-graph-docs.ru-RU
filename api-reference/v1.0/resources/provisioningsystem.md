---
title: тип ресурсов provisioningSystem
description: Представляет систему, в которую пользователь был предварительно или из нее.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d52429fbaa641b1ee0be5208ddf7d85e0830b6c6
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241544"
---
# <a name="provisioningsystem-resource-type"></a>тип ресурсов provisioningSystem

Пространство имен: microsoft.graph


Представляет систему, в которую пользователь был предварительно или из нее. Например, при предоставлении пользователю Azure Active Directory (Azure AD) в ServiceNow, источником системы является Azure AD, а целевой системой является ServiceNow.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|подробности|[detailsInfo](detailsinfo.md)|Сведения о системе.|
|displayName|Строка|Имя системы, в которую пользователь был предварительно или из нее.|
|id|Строка|Идентификатор системы, в которую пользователь был предварительно или из нее.|

## <a name="json-representation"></a>Представление в формате JSON

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


