---
title: тип ресурса unifiedRoleManagementPolicyRuleTarget
description: УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b8b474102e0605fda38db7b0ef39b1105097ba8d5d4b7f376ec3db83e1c07541
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145098"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>тип ресурса unifiedRoleManagementPolicyRuleTarget

Пространство имен: microsoft.graph

УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|вызываемая|Строка|Вызываемая цель правила политики. Допустимые значения: `None` `Admin` , `EndUser` .|
|enforcedSettings|Коллекция String|Список параметров, которые применяются и не могут быть переопределены в детских сферах. Используйте `All` для всех параметров.|
|inheritableSettings|Коллекция String|Список параметров, которые могут наследоваться по детским сферам. Используйте `All` для всех параметров.|
|уровень|String|Уровень целевого показателя правила политики. Допустимые значения: `Eligibility` , `Assignment` .    |
|operations|Коллекция String|Операции для целевой цели правила политики. Допустимые значения: `All` , , , , , `Activate` `Deactivate` `Assign` `Update` `Remove` `Extend` `Renew` .|

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

