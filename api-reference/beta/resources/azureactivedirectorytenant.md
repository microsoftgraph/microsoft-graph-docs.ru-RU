---
title: тип ресурса azureActiveDirectoryTenant
description: Тип azureActiveDirectoryTenant определяет другого клиента Azure Active Directory как источник удостоверений для связанной организации.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9aeb699065a1e4bdf37dfd5f5a90985c47db24f7
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650603"
---
# <a name="azureactivedirectorytenant-resource-type"></a>тип ресурса azureActiveDirectoryTenant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md) Это значение указывает, что этот тип определяет другого клиента Azure Active Directory как источник удостоверений `@odata.type` `#microsoft.graph.azureActiveDirectoryTenant` для связанной организации.

При [](../api/entitlementmanagement-post-connectedorganizations.md)создании новой подключеннойорганизации, если вызывающий вызов предоставляет в коллекции identitySources домен DomainIdentitySource и домен соответствует зарегистрированным доменам клиента Azure Active Directory, то создаемая подключеннаяорганизация будет иметь коллекцию identitySources, содержащую одного члена типа [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| displayName |Строка | Имя клиента Azure Active Directory. Только для чтения. |
| tenantId |String | ID клиента Azure Active Directory клиента. Только для чтения. |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже приводится представление JSON этого типа.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "azureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


