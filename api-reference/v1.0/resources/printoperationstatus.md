---
title: тип ресурса printOperationStatus
description: Представляет текущее состояние длительной операции универсальной печати.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: dd5e7e912ea6810a4a0d501d47a8711830e91ae0
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944895"
---
# <a name="printoperationstatus-resource-type"></a>тип ресурса printOperationStatus

Пространство имен: microsoft.graph

Представляет текущее состояние длительной операции универсальной печати.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|printOperationProcessingState|Текущее состояние обработки printOperation. Допустимые значения описаны в следующей таблице. Только для чтения.|
|description|String|Описание текущего состояния обработки printOperation с читаемым человеком. Только для чтения.|

### <a name="printoperationprocessingstate-values"></a>значения printOperationProcessingState

|Элемент|Значение|Описание|
|:---|:---|:---|
|notStarted|0|Операция еще не началась.|
|запуск|1|Операция запущена.|
|успешно|2|Операция выполнена успешно.|
|не удалось|3|Сбой операции.|
|unknownFutureValue|4|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printOperationStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperationStatus",
  "state": "String",
  "description": "String"
}
```

