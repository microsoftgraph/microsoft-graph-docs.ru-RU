---
title: тип ресурса azureActiveDirectoryTenant
description: Тип azureActiveDirectoryTenant определяет другого клиента Azure Active Directory как источник удостоверений для связанной организации.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 35c517d23b59756d59412e5b898e6b222cc0f8db
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242913"
---
# <a name="azureactivedirectorytenant-resource-type"></a>тип ресурса azureActiveDirectoryTenant

Пространство имен: microsoft.graph


Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md) Это значение указывает, что этот тип определяет другого клиента Azure Active Directory как источник удостоверений `@odata.type` `#microsoft.graph.azureActiveDirectoryTenant` для связанной организации.

При [](../api/entitlementmanagement-post-connectedorganizations.md)создании новой подключеннойорганизации, если вызывающий вызов предоставляет в коллекции identitySources домен DomainIdentitySource и домен соответствует зарегистрированным доменам клиента Azure Active Directory, то создаемая подключеннаяорганизация будет иметь коллекцию identitySources, содержащую одного члена типа [azureActiveDirectoryTenant.](azureactivedirectorytenant.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя клиента Azure Active Directory. Только для чтения. |
|tenantId|String|ID клиента Azure Active Directory клиента. Только для чтения. |

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
  "tenantId": "String",
  "displayName": "String"
}
```



