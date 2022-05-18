---
title: Тип ресурса unifiedRoleManagementPolicyRule
description: Абстрактный тип, который определяет правила или параметры, связанные с политиками управления ролами.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 54444e25d6967536fa2e9a444fd05adf66467881
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461263"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyRule

Пространство имен: microsoft.graph


Абстрактный тип, который определяет правила или параметры, связанные с политиками управления ролами. Этот абстрактный тип наследуется следующими ресурсами, которые определяют различные типы правил и их параметры, связанные с политиками управления ролами.
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
|id|Строка|Идентификатор правила. Наследуется от [сущности](../resources/entity.md). Только для чтения.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)| Определяет сведения об области, на которую нацелено правило политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Отношения
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

