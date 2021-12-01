---
title: тип ресурса domainIdentitySource
description: Тип domainIdentitySource определяет домен, не связанный с клиентом, в качестве источника удостоверений для связанной организации.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6fe969759e07e14af08d3d69e90726dce8512445
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242805"
---
# <a name="domainidentitysource-resource-type"></a>тип ресурса domainIdentitySource

Пространство имен: microsoft.graph


Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md) Это значение указывает на то, что этот тип определяет домен как источник удостоверений `@odata.type` `#microsoft.graph.domainIdentitySource` для связанной организации.

При [](../api/entitlementmanagement-post-connectedorganizations.md)создании новой подключеннойорганизации, если вызывающий вызов предоставляет в коллекции identitySources домен DomainIdentitySource и домен соответствует зарегистрированным доменам клиента Azure Active Directory, то создаемая подключеннаяорганизация будет иметь коллекцию identitySources, содержащую одного члена типа [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя источника удостоверений, как правило, также доменное имя. Только для чтения. |
|domainName|String|Доменное имя. Только для чтения. |

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.domainIdentitySource",
  "domainName": "String",
  "displayName": "String"
}
```

