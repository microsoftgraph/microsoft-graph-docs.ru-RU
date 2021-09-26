---
title: тип ресурса cloudPcManagementGroupAssignmentTarget
description: 'Сложный тип, который представляет целевую группу назначения. Базовый тип: CloudPcManagementAssignmentTarget'
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a3841cc775b1b0ed9221d193a5ca5d44c61bc6f0
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765664"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>тип ресурса cloudPcManagementGroupAssignmentTarget

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, который представляет целевую группу назначения.
Наследует [от cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|groupId|String|ID целевой группы назначения|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.cloudPcManagementAssignmentTarget",
  "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcManagementGroupAssignmentTarget",
  "groupId": "String"
}
```
