---
title: тип ресурса принтера
description: Представляет физическое устройство принтера, зарегистрированное в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d90bf05b77c8843fc9fa5e5f32ecae29ffdaf48e
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765918"
---
# <a name="printer-resource-type"></a>тип ресурса принтера

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройство принтера, зарегистрированное в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.

Этот ресурс поддерживает:
* [Подписка на изменение уведомлений.](/graph/universal-print-webhook-notifications)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создание (регистрация) нового принтера с универсальной печатью. |
| [Get](../api/printer-get.md) | [printer](printer.md) | Ознакомьтесь с свойствами и отношениями объекта принтера. |
| [Обновление](../api/printer-update.md) | [printer](printer.md) | Обновление объекта принтера. |
| [Delete](../api/printer-delete.md) | Нет | Отрегистрим физический принтер из службы универсальной печати. |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | Нет | Восстановление параметров по умолчанию принтера до значений, заданных производителем. |
| [Список заданий](../api/printer-list-jobs.md) | [коллекция printJob](printjob.md) | Получите список заданий печати, которые в очереди для обработки принтером. |
| [Создание задания](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создайте новое задание печати для принтера. Чтобы приступить к печати задания, используйте [start](../api/printjob-start.md). |
| [Перечисление соединителей](../api/printer-list-connectors.md) | [коллекция printConnector](printconnector.md) | Получите список соединитений, с которые связан этот принтер. |
| [Перечисление taskTriggers](../api/printer-list-tasktriggers.md) | Нет | Список [printTaskTriggers, связанных](printtasktrigger.md) с этим принтером. |
| [Создание taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | Создайте [printTaskTrigger,](printtasktrigger.md) который запускается при печатных событиях. |
| [Удаление taskTrigger](../api/printer-delete-tasktrigger.md) | Нет | Удалите [печатьTaskTrigger,](printtasktrigger.md) связанную с принтером. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор принтера. Только для чтения.|
|displayName|String|Имя принтера.|
|manufacturer|String|Производитель сообщил на принтере.|
|model|String|Имя модели, о чем сообщает принтер.|
|registeredDateTime|DateTimeOffset|DateTimeOffset при регистрации принтера. Только для чтения.|
|status|[printerStatus](printerstatus.md)|Состояние обработки принтера, включая ошибки.|
|IsShared|Boolean|True, если принтер является общим; false в противном случае. Только для чтения.|
|hasPhysicalDevice|Логический|True, если на принтере есть физическое устройство для печати. Только для чтения.|
|isAcceptingJobs|Логический|Принимает ли принтер новые задания печати.|
|расположение|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение принтера.|
|defaults|[printerDefaults](printerdefaults.md)|Параметры печати принтера по умолчанию.|
|capabilities|[printerCapabilities](printercapabilities.md)|Возможности принтера.|
|lastSeenDateTime|DateTimeOffset|Самая недавняя датаTimeOffset при взаимодействии принтера с универсальной печатью. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|jobs|[коллекция printJob](printjob.md)| Список заданий, которые в очереди для печати принтером.|
|shares|[коллекция printerShare](printershare.md)| Список принтеров, связанных с принтером. В настоящее время только один принтер Может быть связан с принтером. Только для чтения. Допускается значение null.|
|соединители|[printConnector](printconnector.md)|Соединители, связанные с принтером.|
|taskTriggers|[printTaskTrigger](printtasktrigger.md) collection|Список триггеров задач, связанных с принтером.|

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
  "hasPhysicalDevice": true,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"},
  "lastSeenDateTime": "String (timestamp)"
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


