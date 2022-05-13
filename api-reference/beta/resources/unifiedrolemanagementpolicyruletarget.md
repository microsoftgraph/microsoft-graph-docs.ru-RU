---
title: Тип ресурса unifiedRoleManagementPolicyRuleTarget
description: UnifiedRoleManagementPolicyRuleTarget указывает целевой объект, связанный с политикой управления ролями.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9681efd333a4ea8db98d7a99f481c473dae3c6fb
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399119"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyRuleTarget

Пространство имен: microsoft.graph

UnifiedRoleManagementPolicyRuleTarget указывает целевой объект, связанный с политикой управления ролями.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Вызывающий объект|String|Вызывающий объект для целевого объекта правила политики. Допустимые значения: `None`, `Admin`, `EndUser`.|
|enforcedSettings|Коллекция String|Список параметров, которые применяются и не могут быть переопределены дочерними областями. Используйте `All` для всех параметров.|
|inheritableSettings|Коллекция String|Список параметров, которые могут наследоваться дочерними областями. Используйте `All` для всех параметров.|
|Уровень|String|Уровень для целевого объекта правила политики. Допустимые значения: `Eligibility`, `Assignment`.    |
|operations|Коллекция String|Операции для целевого объекта правила политики. Допустимые значения: `All`, `Activate`, , `Deactivate`, `Assign`, `Update`, `Extend``Remove``Renew`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|targetObjects|Коллекция [directoryObject](../resources/directoryobject.md)|Коллекция пользователей, групп и servicePrincipals, которые находятся в области действия политики. Если этот параметр не указан, все объекты находятся в области действия политики.|

## <a name="json-representation"></a>Представление в формате JSON
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

