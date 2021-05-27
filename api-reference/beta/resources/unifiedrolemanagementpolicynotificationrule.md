---
title: тип ресурса unifiedRoleManagementPolicyNotificationRule
description: В единойroleManagementPolicyNotificationRule указывается правило уведомлений, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c4392055d199e444acefa497a009cf5b71cb8cda
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680201"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>тип ресурса unifiedRoleManagementPolicyNotificationRule

Пространство имен: microsoft.graph

В единойroleManagementPolicyNotificationRule указывается правило уведомлений, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.

Наследует [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для правила. Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|notificationLevel|String|Уровень уведомления. Один из "Нет", "Критический", "Все".|
|notificationRecipients|Коллекция строк|Список уведомлений перекликается с электронной почтой.|
|notificationType|String|Тип уведомления. Одно из сообщений электронной почты.|
|recipientType|String|Тип получателя. Один из requestor, Approver, Admin.|
|isDefaultRecipientsEnabled|Boolean|Получает ли получатель электронной почты по умолчанию или нет.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Цель правила. Унаследованный от [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

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

