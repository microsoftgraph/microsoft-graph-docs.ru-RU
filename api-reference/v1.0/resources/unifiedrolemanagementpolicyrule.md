---
title: Тип ресурса unifiedRoleManagementPolicyRule
description: Абстрактный тип, который определяет правила, связанные с политиками управления ролами.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1ef9d1e4998a46f503b8960c2c0c9fca452a5c08
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246981"
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
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)| Определяет сведения об области, на которую нацелено правило политики управления ролами. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Поддерживает `$filter` (`eq`, `ne`).|

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

