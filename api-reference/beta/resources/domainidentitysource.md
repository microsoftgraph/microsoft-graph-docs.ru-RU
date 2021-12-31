---
title: тип ресурса domainIdentitySource
description: Тип domainIdentitySource определяет домен, не связанный с клиентом, в качестве источника удостоверений для связанной организации.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 392aabbdffd0a9d1a00669e5db1f765503fafd71
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651227"
---
# <a name="domainidentitysource-resource-type"></a>тип ресурса domainIdentitySource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md) Это значение указывает на то, что этот тип определяет домен как источник удостоверений `@odata.type` `#microsoft.graph.domainIdentitySource` для связанной организации.

При [](../api/entitlementmanagement-post-connectedorganizations.md)создании новой подключеннойорганизации, если вызывающий вызов предоставляет в коллекции identitySources домен DomainIdentitySource и домен соответствует зарегистрированным доменам клиента Azure Active Directory, то создаемая подключеннаяорганизация будет иметь коллекцию identitySources, содержащую одного члена типа [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)

## <a name="properties"></a>Свойства

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| displayName |Строка | Имя источника удостоверений, как правило, также доменное имя. Только для чтения. |
| domainName |String | Доменное имя. Только для чтения. |

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже приводится представление JSON этого типа.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


