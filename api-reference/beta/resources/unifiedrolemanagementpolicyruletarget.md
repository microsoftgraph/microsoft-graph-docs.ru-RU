---
title: тип ресурса unifiedRoleManagementPolicyRuleTarget
description: УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9dafa17179d5c2dbecc3446f56c146bdffcf0922
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767239"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>тип ресурса unifiedRoleManagementPolicyRuleTarget

Пространство имен: microsoft.graph

УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|вызываемая|String|Вызываемая цель правила политики. Допустимые значения: `None` `Admin` , `EndUser` .|
|enforcedSettings|Коллекция объектов string|Список параметров, которые применяются и не могут быть переопределены в детских сферах. Используйте `All` для всех параметров.|
|inheritableSettings|Коллекция объектов string|Список параметров, которые могут наследоваться по детским сферам. Используйте `All` для всех параметров.|
|уровень|String|Уровень целевого показателя правила политики. Допустимые значения: `Eligibility` , `Assignment` .    |
|operations|Коллекция объектов string|Операции для целевой цели правила политики. Допустимые значения: `All` , , , , , `Activate` `Deactivate` `Assign` `Update` `Remove` `Extend` `Renew` .|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|targetObjects|Коллекция [directoryObject](../resources/directoryobject.md)|Коллекция пользователей, групп и servicePrincipals, которые находятся в области политики. Если не указано, все объекты находятся в области политики.|

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

