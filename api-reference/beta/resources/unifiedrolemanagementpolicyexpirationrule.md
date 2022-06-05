---
title: Тип ресурса unifiedRoleManagementPolicyExpirationRule
description: Тип, производный от типа ресурса unifiedRoleManagementPolicyRule, который определяет максимальную длительность, которую роль может быть назначена субъекту (посредством прямого назначения или активации соответствия).
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: db7e7956598c27a10a5aab7f6810cf72202f8afd
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898555"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a>Тип ресурса unifiedRoleManagementPolicyExpirationRule

Пространство имен: microsoft.graph

Тип, производный от типа ресурса [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) , который определяет максимальную продолжительность назначения роли субъекту (посредством прямого назначения или активации допустимого значения).

## <a name="methods"></a>Методы

Нет.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор правила. Наследуется от [сущности](../resources/entity.md).|
|isExpirationRequired|Boolean|Указывает, требуется ли срок действия, является ли это постоянно активным назначением или допустимостью. |
|maximumDuration|Длительность| Максимальная длительность, допустимая для допустимости или назначения, которая не является постоянной. Требуется, если **isExpirationRequired** имеет значение `true`. |
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Определяет сведения об области, на которую нацелено правило истечения срока действия. Сведения могут включать тип субъекта, тип назначения роли и действия, влияющие на роль. Наследуется [от unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Поддерживает `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isExpirationRequired": "Boolean",
  "maximumDuration": "String (duration)"
}
```

