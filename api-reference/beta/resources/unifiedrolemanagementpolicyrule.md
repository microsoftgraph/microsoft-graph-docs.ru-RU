---
title: Тип ресурса unifiedRoleManagementPolicyRule
description: UnifiedRoleManagementPolicyRule указывает правило, связанное с политикой управления ролем. Он абстрактный.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d8dee3e3e6b28668b1370a2bb0c34f58e28c82ef
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461312"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyRule

Пространство имен: microsoft.graph

UnifiedRoleManagementPolicyRule указывает правило, связанное с политикой управления ролем. Он абстрактный.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление unifiedRoleManagementPolicyRules](../api/unifiedrolemanagementpolicy-list-rules.md)|[Коллекция unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Получение списка объектов [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) и их свойств.|
|[Получение unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Чтение свойств и связей объекта [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) .|
|[Обновление unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-update.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Обновление свойств объекта [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор правила.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Целевой объект для правила политики.|

## <a name="relationships"></a>Отношения
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

