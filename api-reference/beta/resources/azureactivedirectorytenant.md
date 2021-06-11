---
title: тип ресурса azureActiveDirectoryTenant
description: Тип azureActiveDirectoryTenant определяет другого клиента Azure Active Directory как источник удостоверений для связанной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d7a36c8c737866b20585518e1dc34e6944c97885
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896587"
---
# <a name="azureactivedirectorytenant-resource-type"></a>тип ресурса azureActiveDirectoryTenant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md) Это значение указывает, что этот тип определяет другого клиента Azure Active Directory как источник удостоверений `@odata.type` `#microsoft.graph.azureActiveDirectoryTenant` для связанной организации.

При [](../api/connectedorganization-post.md)создании новой подключеннойорганизации, если вызывающий вызов предоставляет в коллекции identitySources домен DomainIdentitySource и домен соответствует зарегистрированным доменам клиента Azure Active Directory, то создаемая подключеннаяорганизация будет иметь коллекцию identitySources, содержащую одного члена типа [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| displayName |String | Имя клиента Azure Active Directory. Только для чтения. |
| tenantId |String | ID клиента Azure Active Directory клиента. Только для чтения. |

## <a name="relationships"></a>Связи

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


