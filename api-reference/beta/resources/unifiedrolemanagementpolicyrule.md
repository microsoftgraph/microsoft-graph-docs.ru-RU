---
title: Тип ресурса unifiedRoleManagementPolicyRule
description: Абстрактный тип, который определяет правила, связанные с политиками управления ролами.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4851f090b4e73ace7de7b86fc85db76555c918fa
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898520"
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
|id|Строка|Идентификатор правила. Наследуется от [сущности](../resources/entity.md). Только для чтения.|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)| **Не реализовано.** Определяет сведения об области, на которую нацелено правило политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Поддерживает `$filter` (`eq`, `ne`).|

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