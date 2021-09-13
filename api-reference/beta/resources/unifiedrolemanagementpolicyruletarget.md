---
title: тип ресурса unifiedRoleManagementPolicyRuleTarget
description: УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c4d7bfb6744c3272e9237590b4d17c5e1d79b0f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074446"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>тип ресурса unifiedRoleManagementPolicyRuleTarget

Пространство имен: microsoft.graph

УнифицированнаяRoleManagementPolicyRuleTarget указывает цель, связанную с политикой управления ролью.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|вызываемая|String|Вызываемая цель правила политики. Допустимые значения: `None` `Admin` , `EndUser` .|
|enforcedSettings|Коллекция String|Список параметров, которые применяются и не могут быть переопределены в детских сферах. Используйте `All` для всех параметров.|
|inheritableSettings|Коллекция String|Список параметров, которые могут наследоваться по детским сферам. Используйте `All` для всех параметров.|
|уровень|String|Уровень целевого показателя правила политики. Допустимые значения: `Eligibility` , `Assignment` .    |
|operations|Коллекция String|Операции для целевой цели правила политики. Допустимые значения: `All` , , , , , `Activate` `Deactivate` `Assign` `Update` `Remove` `Extend` `Renew` .|

## <a name="relationships"></a>Отношения
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

