---
title: Тип ресурса Провисионингсистемдетаилс
description: Представляет систему, в которую были подготовлены пользователи.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6880214614047000fcc5a793faf4be3e5a88a5e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026448"
---
# <a name="provisioningsystemdetails-resource-type"></a>Тип ресурса Провисионингсистемдетаилс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет систему, в которую были подготовлены пользователи. Например, при подготовке пользователя из Azure Active Directory (Azure AD) к ServiceNow система является системой Azure AD, а целевой системой является ServiceNow.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|details|[detailsInfo](detailsinfo.md)|Сведения о системе.|
|displayName|String|Имя системы, в которую были подготовлены пользователи.|
|id|String|Идентификатор системы, в которую были подготовлены пользователи.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystemDetails",
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
  "description": "provisioningSystemDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


