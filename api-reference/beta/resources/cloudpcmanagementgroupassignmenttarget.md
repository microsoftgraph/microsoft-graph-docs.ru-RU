---
title: Тип ресурса Клаудпкманажементграупассигнменттаржет
description: 'Сложный тип, представляющий целевую группу назначения. Базовый тип: Клаудпкманажементассигнменттаржет'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5216b15a97484bf58d2e2d621dbc26435f180be4
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563874"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>Тип ресурса Клаудпкманажементграупассигнменттаржет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, представляющий целевую группу назначения.
Наследуется от [клаудпкманажементассигнменттаржет](../resources/cloudpcmanagementassignmenttarget.md).

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|groupId|String|Идентификатор целевой группы назначения|

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
