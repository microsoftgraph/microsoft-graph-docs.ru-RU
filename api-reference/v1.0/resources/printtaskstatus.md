---
title: тип ресурса printTaskStatus
description: Представляет текущее состояние выполнения printTask.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7f07ee889cb8f04edff66416ebc6ce49f7e7a3ab67a07119170929fdc12cdf8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229019"
---
# <a name="printtaskstatus-resource-type"></a>тип ресурса printTaskStatus

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет текущее состояние выполнения [printTask](printtask.md). 

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|printTaskProcessingState|Текущее состояние обработки [printTask](printtask.md). Допустимые значения описаны в следующей таблице.|
|description|String|Понятное для человека описание текущего состояния обработки [printTask](printtask.md).|

### <a name="printtaskprocessingstate-values"></a>printTaskProcessingState values

|Элемент|Значение|Описание|
|:---|:---|:---|
|ожидание|0|Выполнение задач находится в стадии ожидания.|
|обработка|1|Выполнение задач продолжается.|
|завершено|2|Выполнение задач завершено.|
|прервано|3|Выполнение задач было прервано.|
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

