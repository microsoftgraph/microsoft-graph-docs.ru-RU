---
title: Тип ресурса unifiedRoleManagementPolicyNotificationRule
description: UnifiedRoleManagementPolicyNotificationRule указывает правило уведомления, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 46e7ec80a8abd9058f74e5bdc8ed01d4d9b81eb2
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398807"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyNotificationRule

Пространство имен: microsoft.graph

UnifiedRoleManagementPolicyNotificationRule указывает правило уведомления, связанное с политикой управления ролем. Он является производным от microsoft.graph.unifiedRoleManagementPolicyRule.

Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|notificationLevel|String|Уровень уведомления. Один из них: "Нет", "Критическое", "Все".|
|notificationRecipients|Коллекция String|Список получателей уведомлений, таких как электронная почта.|
|notificationType|String|Тип уведомления. Один из адресов электронной почты.|
|recipientType|String|Тип получателя. Один из инициаторов запроса, утверждающий, администратор.|
|isDefaultRecipientsEnabled|Логическое|Получает ли получатель сообщение электронной почты по умолчанию.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Целевой объект для правила. Наследуется от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "notificationType": "String",
  "recipientType": "String",
  "notificationLevel": "String",
  "isDefaultRecipientsEnabled": true,
  "notificationRecipients": [
    "String"
  ]
}
```

