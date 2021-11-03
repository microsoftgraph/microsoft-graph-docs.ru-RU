---
title: тип ресурса unifiedRoleManagementPolicyRuleTarget
description: УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6906d88c7430391fc1fcaf322c8d19ed72ab65b1
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695190"
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

