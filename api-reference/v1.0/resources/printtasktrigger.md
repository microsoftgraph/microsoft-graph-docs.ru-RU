---
title: тип ресурса printTaskTrigger
description: Определяет условия, при которых будет выполнен новый printTask на основе связанного печатиTaskDefinition.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ca4c5081521c2cbfd6e5ac4185548507f98e577ed2a590ded43d5788dde6cd9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218424"
---
# <a name="printtasktrigger-resource-type"></a>тип ресурса printTaskTrigger

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Определяет условие, при котором будет запускаться новый [printTask](printtask.md) на основе связанного с ним [принтаTaskDefinition.](printtaskdefinition.md)

Дополнительные сведения о том, как использовать этот ресурс для добавления поддержки печати в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Список](../api/printer-list-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) collection | Получите список printTaskTriggers, связанных с определенным [принтером.](printer.md) |
| [Получение](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | Получите печатьTaskTrigger, связанную с определенным [printTask.](printtask.md) |

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

