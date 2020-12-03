---
title: Тип ресурса Клаудпкпровисионингполициассигнмент
description: Назначения политик подготовки Клаудпк
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 06a90efc67b483fed569a4e7029a74dac4f7f9ee
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563718"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>Тип ресурса Клаудпкпровисионингполициассигнмент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенную коллекцию назначений политик подготовки.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор назначения политики подготовки. Только для чтения. Если `target` это группа пользователей, идентификатор отображается как {полициид} _ {groupId}.|
|target|[клаудпкманажементассигнменттаржет](../resources/cloudpcmanagementassignmenttarget.md)|Цель назначения для политики подготовки. В настоящее время для этой политики поддерживается только одна цель — группа пользователей.|

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
