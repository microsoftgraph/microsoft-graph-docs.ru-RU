---
title: Тип ресурса unifiedRoleManagementPolicyEnablementRule
description: Тип, производный от типа ресурса unifiedRoleManagementPolicyRule, который определяет правила для включения назначения, например включение MFA, обоснование назначений или сведения о билетах.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d9a964a31180348c4e2f797f7ce4769965f17708
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134361"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyEnablementRule

Пространство имен: microsoft.graph

Тип, производный от типа ресурса [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) , который определяет правила для включения назначения, например включение MFA, обоснование назначений или сведения о билетах.

## <a name="methods"></a>Методы

Нет.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|enabledRules|Коллекция String|Коллекция правил, включенных для этого правила политики. Например, `MultiFactorAuthentication`и `Ticketing``Justification`.|
|id|String|Идентификатор правила. Наследуется от [сущности](../resources/entity.md).|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Определяет сведения о области, предназначенной для правила включения. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "enabledRules": [
    "String"
  ]
}
```

