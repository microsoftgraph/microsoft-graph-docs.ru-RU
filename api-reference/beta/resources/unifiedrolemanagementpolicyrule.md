---
title: тип ресурса unifiedRoleManagementPolicyRule
description: В единойRoleManagementPolicyRule указывается правило, связанное с политикой управления ролью. Это абстрактно.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa0bc719fe4722692b1ff42861cccede7150780d
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682245"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>тип ресурса unifiedRoleManagementPolicyRule

Пространство имен: microsoft.graph

В единойRoleManagementPolicyRule указывается правило, связанное с политикой управления ролью. Это абстрактно.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список unifiedRoleManagementPolicyRules](../api/unifiedrolemanagementpolicyrule-list.md)|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получите список объектов [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) и их свойств.|
|[Get unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)|
|[Обновление unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-update.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Обновление свойств единого [объектаRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для правила.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Цель правила политики.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```

