---
title: Тип ресурса Printer
description: Представляет физическое устройство печати, зарегистрированное в универсальной службе печати. Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 37c552a1239ee1d374c22be77ba81004cfc92e1f
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993964"
---
# <a name="printer-resource-type"></a>Тип ресурса Printer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройство принтера, зарегистрированное в универсальной службе печати. Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создание (регистрация) нового принтера с универсальной печатью. |
| [получение](../api/printer-get.md); | [Printer](printer.md) | Чтение свойств и связей объекта Printer. |
| [обновление](../api/printer-update.md). | [Printer](printer.md) | Обновление объекта Printer. |
| [удаление](../api/printer-delete.md); | Нет | Отмените регистрацию физического принтера в универсальной службе печати. |
| [ресторефакторидефаултс](../api/printer-restorefactorydefaults.md) | Нет | Восстановите параметры принтера по умолчанию на значения, заданные производителем. |
| [Список заданий](../api/printer-list-jobs.md) | Коллекция [printJob](printjob.md) | Получение списка заданий печати, помещенных в очередь для обработки принтером. |
| [Создание задания](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создание нового задания печати для принтера. Чтобы начать печать задания, используйте [Start](../api/printjob-start.md). |
| [Перечисление соединителей](../api/printer-list-connectors.md) | Коллекция [принтконнектор](printconnector.md) | Получение списка соединителей, с которыми связан этот принтер. |
| [Перечисление taskTriggers](../api/printer-list-tasktriggers.md) | Нет | Список [принттасктригжерс](printtasktrigger.md) , связанных с этим принтером. |
| [Создание taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | Создание [принттасктригжер](printtasktrigger.md) , выполняемого при возникновении событий печати. |
| [Удаление taskTrigger](../api/printer-delete-tasktrigger.md) | Нет | Удаление [принттасктригжер](printtasktrigger.md) , связанного с принтером. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор документа. Только для чтения.|
|displayName|String|Имя принтера.|
|manufacturer|String|Производитель, сообщаемый принтером.|
|model|String|Имя модели, сообщаемое принтером.|
|регистереддатетиме|DateTimeOffset|Значение DateTimeOffset при регистрации принтера. Только для чтения.|
|status|[принтерстатус](printerstatus.md)|Состояние обработки принтера, включая ошибки.|
|IsShared|Boolean|Значение true, если принтер является общим; в противном случае — false. Только для чтения.|
|isAcceptingJobs|Логический|Принимает ли принтер новые задания печати.|
|расположение|[принтерлокатион](printerlocation.md)|Физическое и/или организационное расположение принтера.|
|defaults|[принтердефаултс](printerdefaults.md)|Параметры печати по умолчанию для принтера.|
|capabilities|[принтеркапабилитиес](printercapabilities.md)|Возможности принтера, связанного с этим общим принтером.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|jobs|Коллекция [printJob](printjob.md)| Список заданий, помещенных в очередь на печать принтером.|
|shares|Коллекция [принтершаре](printershare.md)| Список Принтершарес, связанных с принтером. В настоящее время с принтером может быть связан только один Принтершаре. Только для чтения. Допускается значение null.|
|аудиовыход|[принтконнектор](printconnector.md)|Соединители, связанные с принтером.|
|тасктригжерс|Коллекция [принттасктригжер](printtasktrigger.md)|Список триггеров задач, связанных с принтером.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


