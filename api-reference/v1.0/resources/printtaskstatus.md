---
title: тип ресурса printTaskStatus
description: Представляет текущее состояние выполнения printTask.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d0222192b8c4e7a9fe644edbd956a98a5ad899a7
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60946869"
---
# <a name="printtaskstatus-resource-type"></a>тип ресурса printTaskStatus

Пространство имен: microsoft.graph

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
|unknownFutureValue|4|Эволюционирующее значение sentinel. Не следует использовать.|

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

