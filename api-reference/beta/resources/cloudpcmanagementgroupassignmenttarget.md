---
title: Тип ресурса Клаудпкманажементграупассигнменттаржет
description: 'Сложный тип, представляющий целевую группу назначения. Базовый тип: Клаудпкманажементассигнменттаржет'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a6d046452bb3e9944712746ec7ef72914737186
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378637"
---
# <a name="cloudpcmanagementgroupassignmenttarget-resource-type"></a>Тип ресурса Клаудпкманажементграупассигнменттаржет

Пространство имен: microsoft.graph

Сложный тип, представляющий целевую группу назначения.
Наследуется от [клаудпкманажементассигнменттаржет](../resources/cloudpcmanagementassignmenttarget.md).

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
