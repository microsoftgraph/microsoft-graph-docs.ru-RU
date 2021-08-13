---
title: тип ресурса принтера
description: Представляет физическое устройство принтера, зарегистрированное в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 07e160d21696992588642cd904ffe1f2625c1d1af3fec8e3d56d0feaf9f5d372
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178061"
---
# <a name="printer-resource-type"></a>тип ресурса принтера

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет устройство принтера, зарегистрированное в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.

Этот ресурс поддерживает:
* [Подписка на изменение уведомлений.](/graph/universal-print-webhook-notifications)

Наследует от [printerBase](../resources/printerbase.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Создание](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создание (регистрация) нового принтера с универсальной печатью. |
| [Получение](../api/printer-get.md) | [printer](printer.md) | Ознакомьтесь с свойствами и отношениями объекта принтера. |
| [Обновление](../api/printer-update.md) | [printer](printer.md) | Обновление объекта принтера. |
| [Удаление](../api/printer-delete.md) | Нет | Отрегистрим физический принтер из службы универсальной печати. |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | Нет | Восстановление параметров по умолчанию принтера до значений, заданных производителем. |
| [Список заданий](../api/printer-list-jobs.md) | [коллекция printJob](printjob.md) | Получите список заданий печати, которые в очереди для обработки принтером. |
| [Создание задания](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создайте новое задание печати для принтера. Чтобы приступить к печати задания, используйте [start](../api/printjob-start.md). |
| [Перечисление соединителей](../api/printer-list-connectors.md) | [коллекция printConnector](printconnector.md) | Получите список соединитений, с которые связан этот принтер. |
| [Перечисление общих ресурсов](../api/printer-list-shares.md) | [коллекция printerShare](printerShare.md) | Получите список принтеров, с которые связан этот принтер. В настоящее время только один принтер Может быть связан с принтером. |
| [Перечисление taskTriggers](../api/printer-list-tasktriggers.md) | Нет | Список [printTaskTriggers, связанных](printtasktrigger.md) с этим принтером. |
| [Создание taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | Создайте [printTaskTrigger,](printtasktrigger.md) который запускается при печатных событиях. |
| [Удаление taskTrigger](../api/printer-delete-tasktrigger.md) | Нет | Удалите [печатьTaskTrigger,](printtasktrigger.md) связанную с принтером. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор документа. Унаследованный от [printerBase](../resources/printerbase.md). Только для чтения.|
|displayName|String|Имя принтера. Унаследованный от [printerBase](../resources/printerbase.md).|
|manufacturer|String|Производитель сообщил на принтере. Унаследованный от [printerBase](../resources/printerbase.md).|
|model|String|Имя модели, о чем сообщает принтер. Унаследованный от [printerBase](../resources/printerbase.md).|
|registeredDateTime|DateTimeOffset|DateTimeOffset при регистрации принтера. Только для чтения.|
|status|[printerStatus](printerstatus.md)|Состояние обработки принтера, включая ошибки. Унаследованный от [printerBase](../resources/printerbase.md).|
|IsShared|Boolean|True, если принтер является общим; false в противном случае. Только для чтения.|
|hasPhysicalDevice|Логическое|True, если на принтере есть физическое устройство для печати. Только для чтения.|
|isAcceptingJobs|Логическое|Принимает ли принтер новые задания печати. Унаследованный от [printerBase](../resources/printerbase.md).|
|расположение|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение принтера. Унаследованный от [printerBase](../resources/printerbase.md).|
|defaults|[printerDefaults](printerdefaults.md)|Параметры печати принтера по умолчанию. Унаследованный от [printerBase](../resources/printerbase.md).|
|capabilities|[printerCapabilities](printercapabilities.md)|Возможности принтера, связанного с этим разделом принтера. Унаследованный от [printerBase](../resources/printerbase.md).|
|lastSeenDateTime|DateTimeOffset|Самая недавняя датаTimeOffset при взаимодействии принтера с универсальной печатью. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|jobs|[коллекция printJob](printjob.md)| Список заданий, которые в очереди для печати принтером.  Унаследованный от [printerBase](../resources/printerbase.md).|
|shares|[коллекция printerShare](printershare.md)| Список принтеров, связанных с принтером. В настоящее время только один принтер Может быть связан с принтером. Только для чтения. Допускается значение null.|
|соединители|[printConnector](printconnector.md)|Соединители, связанные с принтером.|
|taskTriggers|[printTaskTrigger](printtasktrigger.md) collection|Список триггеров задач, связанных с принтером.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printer",
  "baseType": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printer",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "registeredDateTime": "String (timestamp)",
  "isShared": "Boolean",
  "hasPhysicalDevice": "Boolean",
  "lastSeenDateTime": "String (timestamp)"
}
```

