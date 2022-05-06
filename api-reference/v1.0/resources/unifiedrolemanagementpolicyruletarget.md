---
title: Тип ресурса unifiedRoleManagementPolicyRuleTarget
description: Определяет сведения об области, предназначенной для правила политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f0b796bb00601d33bdeba2bd2acab8277f526f4d
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247254"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyRuleTarget

Пространство имен: microsoft.graph

Определяет сведения об области, предназначенной для правила политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|Вызывающий объект|String|Тип вызывающего объекта, который является целевым объектом правила политики. Допустимые значения: `None`, `Admin`, `EndUser`.|
|enforcedSettings|Коллекция строк|Список параметров роли, которые применяются и не могут быть переопределены дочерними областями. Используйте `All` для всех параметров.|
|inheritableSettings|Коллекция строк|Список параметров роли, которые могут наследоваться дочерними областями. Используйте `All` для всех параметров.|
|Уровень|String|Тип назначения роли, который является целевым объектом правила политики. Допустимые значения: `Eligibility`, `Assignment`.   |
|operations|Коллекция строк|Операции управления ролами, которые являются целью правила политики. Допустимые значения: `All`, `Activate`, , `Deactivate`, `Assign`, `Update`, `Extend``Remove``Renew`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|targetObjects|Коллекция [directoryObject](../resources/directoryobject.md)| **Не реализовано.** Коллекция пользователей, групп и субъектов-служб, которые находятся в области действия политики. Если этот параметр не указан, все объекты находятся в области действия политики.|

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

