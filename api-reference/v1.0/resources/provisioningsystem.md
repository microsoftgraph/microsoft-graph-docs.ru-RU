---
title: тип ресурсов provisioningSystem
description: Представляет систему, в которую пользователь был предварительно или из нее.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b39cccfaf8dd3d064a3065707a96b955f3cd2b22
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078711"
---
# <a name="provisioningsystem-resource-type"></a>тип ресурсов provisioningSystem

Пространство имен: microsoft.graph


Представляет систему, в которую пользователь был предварительно или из нее. Например, при предоставлении пользователю Azure Active Directory (Azure AD) в ServiceNow, источником системы является Azure AD, а целевой системой является ServiceNow.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|details|[detailsInfo](detailsinfo.md)|Сведения о системе.|
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


