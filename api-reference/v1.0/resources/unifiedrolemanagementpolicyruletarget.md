---
title: Тип ресурса unifiedRoleManagementPolicyRuleTarget
description: Определяет сведения об области, предназначенной для правила политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1ae571305de5d7f20635467e65d38090761b21ce
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134425"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyRuleTarget

Пространство имен: microsoft.graph

Определяет сведения об области, предназначенной для правила политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|Вызывающий объект|String|Тип вызывающего объекта, который является целевым объектом правила политики. Допустимые значения: `None`, `Admin`, `EndUser`.|
|enforcedSettings|Коллекция строк|Список параметров роли, которые применяются и не могут быть переопределены дочерними областями. Используйте `All` для всех параметров.|
|inheritableSettings|Коллекция String|Список параметров роли, которые могут наследоваться дочерними областями. Используйте `All` для всех параметров.|
|Уровень|String|Тип назначения роли, который является целевым объектом правила политики. Допустимые значения: `Eligibility`, `Assignment`.   |
|operations|Коллекция String|Операции управления ролами, которые являются целью правила политики. Допустимые значения: `All`, `Activate`, , `Deactivate`, `Assign`, `Update`, `Extend``Remove``Renew`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|targetObjects|Коллекция [directoryObject](../resources/directoryobject.md)| Коллекция пользователей, групп и субъектов-служб, которые находятся в области действия политики. Если этот параметр не указан, все объекты находятся в области действия политики.|

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

