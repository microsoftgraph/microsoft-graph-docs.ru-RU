---
title: тип ресурса cloudPcProvisioningPolicyAssignment
description: Назначения политики подготовка CloudPC
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: fba54fda5ad20142909b7fea7c01bb117e5b3911
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767393"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>тип ресурса cloudPcProvisioningPolicyAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор назначений политики обеспечения.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для назначения политики обеспечения. Только для чтения. Если это группа пользователей, то ID отображается как `target` {policyId} \_ {groupId}.|
|target|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|Цель назначения для политики обеспечения. В настоящее время единственной целью, поддерживаемой для этой политики, является группа пользователей. Подробные сведения см. [в материале cloudPcManagementGroupAssignmentTarget.](cloudpcmanagementgroupassignmenttarget.md) |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
    "groupId": "String"
  }
}
```
