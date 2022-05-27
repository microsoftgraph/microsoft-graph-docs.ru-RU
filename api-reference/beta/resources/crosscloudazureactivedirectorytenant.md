---
title: Тип ресурса crossCloudAzureActiveDirectoryTenant
description: Тип crossCloudAzureActiveDirectoryTenant определяет другой клиент Azure Active Directory в другом облаке в качестве источника удостоверений для подключенной организации.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8086a5311626a520b96146205076b04547c0cfce
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694417"
---
# <a name="crosscloudazureactivedirectorytenant-resource-type"></a>Тип ресурса crossCloudAzureActiveDirectoryTenant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в источниках удостоверений объекта [connectedOrganization](connectedOrganization.md) . Значение `@odata.type` указывает`#microsoft.graph.crossCloudAzureActiveDirectoryTenant`, что этот тип определяет другой клиент Azure AD в другом облаке в качестве источника удостоверений для подключенной организации.


## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| cloudInstance | Строка | Идентификатор облака, в котором находится клиент, один из `microsoftonline.com``microsoftonline.us` `partner.microsoftonline.cn`или . Только для чтения. |
| displayName |Строка | Имя Azure Active Directory клиента. Только для чтения. |
| tenantId |String | Идентификатор клиента Azure Active Directory. Только для чтения. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже приведено представление типа в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.crossCloudAzureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String",
  "cloudInstance": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "crossCloudAzureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


