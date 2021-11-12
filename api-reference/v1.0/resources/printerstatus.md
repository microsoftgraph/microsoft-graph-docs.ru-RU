---
title: тип ресурса printerStatus
description: Представляет состояние обработки принтера, включая все ошибки.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: da2c455f08830ee7bbfdf38def36f03250b21877
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936973"
---
# <a name="printerstatus-resource-type"></a>тип ресурса printerStatus

Пространство имен: microsoft.graph

Представляет состояние обработки принтера, включая все ошибки.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|printerProcessingState|Текущее состояние обработки. Допустимые значения описаны в следующей таблице. Только для чтения.|
|details|коллекция printerProcessingStateDetail|Список сведений, описывающих, почему принтер находится в текущем состоянии. Допустимые значения описаны в следующей таблице. Только для чтения.|
|description|String|Описание текущего состояния обработки принтера, считываемым человеком. Только для чтения.|

### <a name="printerprocessingstate-values"></a>значения printerProcessingState

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние обработки, о чем сообщает принтер, неизвестно.|
|праздный|1|Принтер простаивает и готов к приему новых заданий печати.|
|обработка|2|В настоящее время принтер обрабатывает задание печати и обрабатывает все ожидающие задания по завершении.|
|остановлено|3|Принтер столкнулся с проблемой (например, закончились бумаги в активном лотке) и не может продолжить текущую работу печати до тех пор, пока проблема не будет устранена. Дополнительные **сведения см.** в  дополнительных сведениях о значении (s) или значении описания.|
|unknownFutureValue|4|Эволюционирующее значение sentinel. Не следует использовать.|

### <a name="printerprocessingstatedetail-values"></a>значения printerProcessingStateDetail

[тип enum printerProcessingStateDetail](./printerprocessingstatedetail.md)

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerStatus",
  "state": "String",
  "details": [
    "String"
  ],
  "description": "String"
}
```
