---
title: тип ресурса cloudPcProvisioningPolicyAssignment
description: Назначения политики подготовка CloudPC
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a96c3717b97b3f721c77b1150841f1eb51ded89f
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082246"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>тип ресурса cloudPcProvisioningPolicyAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенный набор назначений политики обеспечения.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

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
