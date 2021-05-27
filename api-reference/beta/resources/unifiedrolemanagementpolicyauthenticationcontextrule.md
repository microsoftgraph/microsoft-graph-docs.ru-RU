---
title: тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule
description: В единойroleManagementPolicyAuthenticationContextRule указывается правило включить, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5e3db8812b58b8276ab2fdd977e110f30a874c9b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680698"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a>тип ресурса unifiedRoleManagementPolicyAuthenticationContextRule

Пространство имен: microsoft.graph

В единойroleManagementPolicyAuthenticationContextRule указывается правило включить, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.

Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|claimValue|String|Значение утверждения контекста проверки подлинности.|
|id|String|Уникальный идентификатор для правила. Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|isEnabled|Boolean|Указывает, включен ли параметр.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Цель правила. Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isEnabled": "Boolean",
  "claimValue": "String"
}
```

