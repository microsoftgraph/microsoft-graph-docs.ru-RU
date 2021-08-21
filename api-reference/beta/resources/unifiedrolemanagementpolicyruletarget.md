---
title: тип ресурса unifiedRoleManagementPolicyRuleTarget
description: УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5efeaacbcc6b8f74d1b1ab7ee9a83cce139721ed
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453620"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>тип ресурса unifiedRoleManagementPolicyRuleTarget

Пространство имен: microsoft.graph

УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|вызываемая|String|Вызываемая цель правила политики. Допустимые значения: `None` `Admin` , `EndUser` .|
|enforcedSettings|Коллекция строк|Список параметров, которые применяются и не могут быть переопределены в детских сферах. Используйте `All` для всех параметров.|
|inheritableSettings|Коллекция строк|Список параметров, которые могут наследоваться по детским сферам. Используйте `All` для всех параметров.|
|уровень|String|Уровень целевого показателя правила политики. Допустимые значения: `Eligibility` , `Assignment` .    |
|operations|Коллекция строк|Операции для целевой цели правила политики. Допустимые значения: `All` , , , , , `Activate` `Deactivate` `Assign` `Update` `Remove` `Extend` `Renew` .|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|targetObjects|Коллекция [directoryObject](../resources/directoryobject.md)|Коллекция пользователей, групп и servicePrincipals, которые находятся в области политики. Если не указано, все объекты находятся в области политики.|
-->
## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
  "caller": "String",
  "operations": [
    "String"
  ],
  "level": "String",
  "inheritableSettings": [
    "String"
  ],
  "enforcedSettings": [
    "String"
  ]
}
```

