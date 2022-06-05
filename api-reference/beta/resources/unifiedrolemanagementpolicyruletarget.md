---
title: Тип ресурса unifiedRoleManagementPolicyRuleTarget
description: Определяет сведения об области, предназначенной для правила политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 47989969bdce1060d01a6e4b300b5df9e16de67a
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899066"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyRuleTarget

Пространство имен: microsoft.graph

Определяет сведения об области, предназначенной для правила политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|Вызывающий объект|Строка|Тип вызывающего объекта, который является целевым объектом правила политики. Допустимые значения: `None`, `Admin`, `EndUser`.|
|enforcedSettings|Коллекция String|Список параметров роли, которые применяются и не могут быть переопределены дочерними областями. Используйте `All` для всех параметров.|
|inheritableSettings|Коллекция объектов string|Список параметров роли, которые могут наследоваться дочерними областями. Используйте `All` для всех параметров.|
|Уровень|Строка|Тип назначения роли, который является целевым объектом правила политики. Допустимые значения: `Eligibility`, `Assignment`.   |
|operations|Коллекция объектов string|Операции управления ролами, которые являются целью правила политики. Допустимые значения: `All`, `Activate`, , `Deactivate`, `Assign`, `Update`, `Extend``Remove``Renew`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|targetObjects|Коллекция [directoryObject](../resources/directoryobject.md)| Коллекция пользователей, групп и субъектов-служб, которые находятся в области действия политики. Если этот параметр не указан, все объекты находятся в области действия политики.|

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