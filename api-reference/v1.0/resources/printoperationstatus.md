---
title: тип ресурса printOperationStatus
description: Представляет текущее состояние длительной операции универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 787a584b32c6f34d78d14fa4d676b1be30a62c25
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517469"
---
# <a name="printoperationstatus-resource-type"></a>тип ресурса printOperationStatus

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет текущее состояние длительной операции универсальной печати.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|state|printOperationProcessingState|Текущее состояние обработки printOperation. Допустимые значения описаны в следующей таблице. Только для чтения.|
|description|Строка|Описание текущего состояния обработки printOperation с читаемым человеком. Только для чтения.|

### <a name="printoperationprocessingstate-values"></a>значения printOperationProcessingState

|Элемент|Значение|Описание|
|:---|:---|:---|
|notStarted|0|Операция еще не началась.|
|запуск|1 |Операция запущена.|
|успешно|2 |Операция выполнена успешно.|
|не удалось|3 |Сбой операции.|
|unknownFutureValue|4 |Эволюционирующее значение sentinel. Не следует использовать.|

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

