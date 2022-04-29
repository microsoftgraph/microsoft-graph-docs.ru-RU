---
title: Тип ресурса unifiedRoleManagementPolicyNotificationRule
description: Тип, производный от типа ресурса unifiedRoleManagementPolicyRule, который определяет правила уведомлений по электронной почте для назначений ролей, активаций и утверждений.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0fae65ed41efb482278af0d3a802c9002b242891
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134357"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyNotificationRule

Пространство имен: microsoft.graph

Тип, производный от типа ресурса [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) , который определяет правила уведомлений по электронной почте для назначений ролей, активаций и утверждений.

Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="methods"></a>Методы

Нет.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор правила. Наследуется от [сущности](../resources/entity.md).|
|isDefaultRecipientsEnabled|Логическое|Указывает, будет ли получатель по умолчанию получать уведомление по электронной почте.|
|notificationLevel|String|Уровень уведомления. Возможные значения: `None`, `Critical`. `All`|
|notificationRecipients|Коллекция String|Список получателей уведомлений по электронной почте.|
|notificationType|String|Тип уведомления. Поддерживается `Email` только.|
|recipientType|String|Тип получателя уведомления. Возможные значения: `Requestor`, `Approver`. `Admin`|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Определяет сведения об области, на которую нацелено правило уведомления. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Поддерживает `$filter` (`eq`, `ne`).|

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
  "isDefaultRecipientsEnabled": "Boolean",
  "notificationRecipients": [
    "String"
  ]
}
```

