---
title: Тип ресурса unifiedRoleManagementPolicyEnablementRule
description: Тип, производный от типа ресурса unifiedRoleManagementPolicyRule, который определяет правила для включения назначения, например включение MFA, обоснование назначений или сведения о билетах.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 512821df715da8b5b2261293ce18233741d67183
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899080"
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
|id|Строка|Идентификатор правила. Наследуется от [сущности](../resources/entity.md).|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Определяет сведения о области, предназначенной для правила включения. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Поддерживает `$filter` (`eq`, `ne`).|


## <a name="relationships"></a>Отношения
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

