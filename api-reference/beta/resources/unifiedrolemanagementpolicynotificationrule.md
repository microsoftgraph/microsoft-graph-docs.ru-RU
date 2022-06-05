---
title: Тип ресурса unifiedRoleManagementPolicyNotificationRule
description: Тип, производный от типа ресурса unifiedRoleManagementPolicyRule, который определяет правила уведомлений по электронной почте для назначений ролей, активаций и утверждений.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a7f70afe8daa0bd296033be244bf2f7370ce1bdd
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898541"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyNotificationRule

Пространство имен: microsoft.graph

Тип, производный от типа ресурса [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) , который определяет правила уведомлений по электронной почте для назначений ролей, активаций и утверждений.

Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор правила. Наследуется от [сущности](../resources/entity.md).|
|isDefaultRecipientsEnabled|Boolean|Указывает, будет ли получатель по умолчанию получать уведомление по электронной почте.|
|notificationLevel|Строка|Уровень уведомления. Возможные значения: `None`, `Critical`. `All`|
|notificationRecipients|Коллекция String|Список получателей уведомлений по электронной почте.|
|notificationType|Строка|Тип уведомления. Поддерживается `Email` только.|
|recipientType|Строка|Тип получателя уведомления. Возможные значения: `Requestor`, `Approver`. `Admin`|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Определяет сведения об области, на которую нацелено правило уведомления. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Отношения
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