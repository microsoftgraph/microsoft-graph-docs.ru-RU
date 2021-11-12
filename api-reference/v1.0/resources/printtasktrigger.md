---
title: тип ресурса printTaskTrigger
description: Определяет условия, при которых будет выполнен новый printTask на основе связанного печатиTaskDefinition.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b458b99c08a945198ddd1cd21678e0513a85a8b5
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944258"
---
# <a name="printtasktrigger-resource-type"></a>тип ресурса printTaskTrigger

Пространство имен: microsoft.graph

Определяет условие, при котором будет запускаться новый [printTask](printtask.md) на основе связанного с ним [принтаTaskDefinition.](printtaskdefinition.md)

Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Список](../api/printer-list-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) collection | Получите список printTaskTriggers, связанных с определенным [принтером.](printer.md) |
| [Получение](../api/printtasktrigger-get.md); | [printTaskTrigger](printtasktrigger.md) | Получите печатьTaskTrigger, связанную с определенным [printTask.](printtask.md) |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор printTaskTrigger. Только для чтения.|
|event|printEvent|Событие Universal Print, которое приведет к запуску новой [печатиTask.](printtask.md) Допустимые значения описаны в следующей таблице.|

### <a name="printevent-values"></a>printEvent values

|Элемент|Значение|Описание|
|:---|:---|:---|
|jobStarted|0|Представляет событие, которое происходит при работе с новой печатью.|
|unknownFutureValue|1|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определение|[printTaskDefinition](printtaskdefinition.md)|Абстрактное определение, которое будет использоваться для создания [printTask](printtask.md) при запуске события печати. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskTrigger",
  "id": "String (identifier)",
  "event": "String"
}
```

