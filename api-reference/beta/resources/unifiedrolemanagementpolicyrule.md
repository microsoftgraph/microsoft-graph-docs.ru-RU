---
title: тип ресурса unifiedRoleManagementPolicyRule
description: В единойRoleManagementPolicyRule указывается правило, связанное с политикой управления ролью. Это абстрактно.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 27b982cb74dfac20f14377a2751a0aabb9756830
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64508680"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>тип ресурса unifiedRoleManagementPolicyRule

Пространство имен: microsoft.graph

В единойRoleManagementPolicyRule указывается правило, связанное с политикой управления ролью. Это абстрактно.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список unifiedRoleManagementPolicyRules](../api/unifiedrolemanagementpolicyrule-list.md)|[коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получите список объектов [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) и их свойств.|
|[Get unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Ознакомьтесь с свойствами и отношениями объекта [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) .|
|[Обновление unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-update.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Обновление свойств единого [объектаRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для правила.|
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

