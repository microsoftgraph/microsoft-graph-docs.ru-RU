---
title: тип ресурса unifiedRoleManagementPolicyNotificationRule
description: В единойroleManagementPolicyNotificationRule указывается правило уведомлений, связанное с политикой управления ролью. Она получена из microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bcf4a9dca524f1c0d8c36328df5c140e0bedb47c0d1fb56d871dd7942d9fb80a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145119"
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
|notificationRecipients|Коллекция String|Список уведомлений перекликается с электронной почтой.|
|notificationType|Строка|Тип уведомления. Одно из сообщений электронной почты.|
|recipientType|Строка|Тип получателя. Один из requestor, Approver, Admin.|
|isDefaultRecipientsEnabled|Логический|Получает ли получатель электронной почты по умолчанию или нет.|
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

