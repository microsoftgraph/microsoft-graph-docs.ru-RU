---
title: тип ресурса printTaskStatus
description: Представляет текущее состояние выполнения printTask.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ef5587050926fef5fa924f6d541de63d5b1d33aa
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518017"
---
# <a name="printtaskstatus-resource-type"></a>тип ресурса printTaskStatus

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет текущее состояние выполнения [printTask](printtask.md). 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|printTaskProcessingState|Текущее состояние обработки [printTask](printtask.md). Допустимые значения описаны в следующей таблице.|
|description|Строка|Понятное для человека описание текущего состояния обработки [printTask](printtask.md).|

### <a name="printtaskprocessingstate-values"></a>printTaskProcessingState values

|Элемент|Значение|Описание|
|:---|:---|:---|
|ожидание|0|Выполнение задач находится в стадии ожидания.|
|обработка|1 |Выполнение задач продолжается.|
|завершено|2 |Выполнение задач завершено.|
|прервано|3 |Выполнение задач было прервано.|
|unknownFutureValue|4 |Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printTaskStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskStatus",
  "state": "String",
  "description": "String"
}
```

