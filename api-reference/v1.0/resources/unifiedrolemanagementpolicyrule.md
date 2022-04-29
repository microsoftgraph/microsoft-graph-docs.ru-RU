---
title: Тип ресурса unifiedRoleManagementPolicyRule
description: Абстрактный тип, который определяет правила, связанные с политиками управления ролами.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 06db472f1af4634d409f51afb788dfca80d33dda
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134428"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyRule

Пространство имен: microsoft.graph


Абстрактный тип, который определяет правила, связанные с политиками управления ролами. Этот абстрактный тип наследуется следующими ресурсами, которые определяют различные типы правил и их параметры, связанные с политиками управления ролами.
+ [unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md)
+ [unifiedRoleManagementPolicyAuthenticationContextRule](unifiedrolemanagementpolicyauthenticationcontextrule.md)
+ [unifiedRoleManagementPolicyEnablementRule](unifiedrolemanagementpolicyenablementrule.md)
+ [unifiedRoleManagementPolicyExpirationRule](unifiedrolemanagementpolicyexpirationrule.md)
+ [unifiedRoleManagementPolicyNotificationRule](unifiedrolemanagementpolicynotificationrule.md)


Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор правила. Наследуется от [сущности](../resources/entity.md). Только для чтения.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)| **Не реализовано.** Определяет сведения об области, на которую нацелено правило политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "baseType": "microsoft.graph.entity",
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

