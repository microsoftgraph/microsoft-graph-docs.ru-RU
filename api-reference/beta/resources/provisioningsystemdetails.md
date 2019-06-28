---
title: Тип ресурса Провисионингсистемдетаилс
description: Представляет систему, в которую были подготовлены пользователи.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e84af77ac7d2b14fb25ce07939bc1a542102fb19
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349447"
---
# <a name="provisioningsystemdetails-resource-type"></a>Тип ресурса Провисионингсистемдетаилс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет систему, в которую были подготовлены пользователи. Например, при подготовке пользователя из Azure Active Directory (Azure AD) к ServiceNow система является системой Azure AD, а целевой системой является ServiceNow.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|details|[Детаилсинфо](detailsinfo.md)|Сведения о системе.|
|displayName|Строка|Имя системы, в которую были подготовлены пользователи.|
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
