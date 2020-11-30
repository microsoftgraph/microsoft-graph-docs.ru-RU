---
title: Тип ресурса Клаудпкпровисионингполициассигнмент
description: Назначения политик подготовки Клаудпк
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbbdf76dfb184efdae7279b5d4970367995c0a6c
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378566"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>Тип ресурса Клаудпкпровисионингполициассигнмент

Пространство имен: microsoft.graph

Представляет определенную коллекцию назначений политик подготовки.


## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор назначения политики подготовки. Только для чтения. Если `target` это группа пользователей, идентификатор отображается как {полициид} _ {groupId}.|
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
