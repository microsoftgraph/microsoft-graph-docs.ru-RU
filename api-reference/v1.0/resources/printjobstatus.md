---
title: тип ресурса printJobStatus
description: Представляет текущее состояние задания печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7a6f5e0c728c1de122f9b642b9de2f1db050cf09
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518061"
---
# <a name="printjobstatus-resource-type"></a>тип ресурса printJobStatus

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет текущее состояние задания печати.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|printJobProcessingState|Текущее состояние обработки задания печати. Допустимые значения описаны в следующей таблице. Только для чтения.|
|details|printJobProcessingDetail collection|Дополнительные сведения для состояния задания печати. Допустимые значения описаны в следующей таблице. Только для чтения.|
|description|Строка|Описание текущего состояния обработки задания печати, считываемым человеком. Только для чтения.|
|isAcquiredByPrinter|Логический|True, если задание было признано принтером; false в противном случае. Только для чтения.|

### <a name="printjobprocessingstate-values"></a>printJobProcessingState values

|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние обработки, о чем сообщает принтер, не распознается.|
|ожидание|1 |Задание печати находится в ожидании обработки принтером.|
|обработка|2 |Задание печати в настоящее время обрабатывается принтером.|
|приостановлено|3 |Задание печати приостановлено.|
|остановлено|4 |Задание печати было остановлено, так как перед продолжением работы необходимо устранить проблему с принтером. Дополнительные сведения можно найти на ресурсе состояния принтера.|
|завершено|5 |Задание печати выполнено успешно, и дальнейшая обработка не будет выполнена.|
|отменено|6 |Задание печати было отменено пользователем, и дальнейшая обработка не будет происходить.|
|прервано|7 |Задание печати было прервано пользователем или принтером, и дальнейшая обработка не будет происходить.|

### <a name="printjobprocessingdetail-values"></a>printJobProcessingDetail values

|Элемент|Значение|Описание|
|:---|:---|:---|
|uploadPending|0|Загрузка полезной нагрузки документа не была.|
|преобразование|1 |Преобразование полезной нагрузки документа.|
|completedSuccessfully|2 |Задание выполнено успешно.|
|completedWithWarnings|3 |Задание выполнено с помощью предупреждений.|
|completedWithErrors|4 |Задание выполнено с ошибками.|
|releaseWait|5 |Ожидается, что задание будет выпущено.|
|интерпретация|6 |Задание находится в состоянии "обработка", но, более конкретно, документ полезной нагрузки в настоящее время интерпретируется.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobStatus",
  "state": "String",
  "description": "String",
  "isAcquiredByPrinter": "Boolean",
  "details": [
    "String"
  ]
}
```

