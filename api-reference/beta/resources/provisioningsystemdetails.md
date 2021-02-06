---
title: Тип ресурса provisioningSystemDetails
description: Представляет систему, для которую пользователь был представлен или из нее.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5400088c1f239bd73e093679bbc13b8034800f28
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135340"
---
# <a name="provisioningsystemdetails-resource-type"></a>Тип ресурса provisioningSystemDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет систему, для которую пользователь был представлен или из нее. Например, при подготовка пользователя из Azure Active Directory (Azure AD) в ServiceNow, источником системы является Azure AD, а целевая система — ServiceNow.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|details|[detailsInfo](detailsinfo.md)|Сведения о системе.|
|displayName|Строка|Имя системы, в которую или из нее был вошел пользователь.|
|id|Строка|Идентификатор системы, в которую или из нее был вошел пользователь.|

## <a name="json-representation"></a>Представление в формате JSON

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


