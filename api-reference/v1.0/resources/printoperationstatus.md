---
title: тип ресурса printOperationStatus
description: Представляет текущее состояние длительной операции универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 968958ef9d016b672bfe4d100cfc09f7a3b57d6c6c3ff28c36309ec6df04fe4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54154891"
---
# <a name="printoperationstatus-resource-type"></a>тип ресурса printOperationStatus

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

