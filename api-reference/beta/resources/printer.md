---
title: Тип ресурса printer
description: Представляет физическое принтерное устройство, зарегистрированное в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fab3e933608143846555c556a215025e39666257
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934875"
---
# <a name="printer-resource-type"></a>Тип ресурса printer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет принтер, зарегистрированный в службе универсальной печати. Ресурсы принтера можно использовать для управления заданиями печати, настройками принтера, метаданными принтера и состоянием регистрации.

Этот ресурс поддерживает:
* [Подписка на уведомления об изменениях.](/graph/universal-print-webhook-notifications)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создайте (зарегистрируйте) новый принтер с помощью универсальной печати. |
| [получение](../api/printer-get.md); | [printer](printer.md) | Чтение свойств и связей объекта принтера. |
| [обновление](../api/printer-update.md). | [printer](printer.md) | Обновление объекта принтера. |
| [удаление](../api/printer-delete.md); | Нет | Отостересть физического принтера от службы универсальной печати. |
| [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md) | Нет | Восстановите параметры принтера по умолчанию до значений, указанных производителем. |
| [Список заданий](../api/printer-list-jobs.md) | [Коллекция printJob](printjob.md) | Получите список заданий печати, которые находятся в очереди для обработки принтером. |
| [Создание задания](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создайте новое задание печати для принтера. Чтобы начать печать задания, [используйте](../api/printjob-start.md)start . |
| [Перечисление соединителей](../api/printer-list-connectors.md) | [Коллекция printConnector](printconnector.md) | Получите список соединитений, с которые связан этот принтер. |
| [Перечисление taskTriggers](../api/printer-list-tasktriggers.md) | Нет | Список [printTaskTriggers,](printtasktrigger.md) связанных с этим принтером. |
| [Создание taskTrigger](../api/printer-post-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) | Создайте [printTaskTrigger,](printtasktrigger.md) который запускается при событиях печати. |
| [Удаление taskTrigger](../api/printer-delete-tasktrigger.md) | Нет | Удалите [printTaskTrigger,](printtasktrigger.md) связанный с принтером. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор документа. Только для чтения.|
|displayName|String|Имя принтера.|
|manufacturer|String|Изготовитель, о чем сообщил принтер.|
|model|String|Имя модели, сообщаемая принтером.|
|registeredDateTime|DateTimeOffset|DateTimeOffset при регистрации принтера. Только для чтения.|
|status|[printerStatus](printerstatus.md)|Состояние обработки принтера, включая все ошибки.|
|IsShared|Boolean|Имеет true, если принтер является общим; в противном случае false. Только для чтения.|
|hasPhysicalDevice|Boolean|Имеет true, если принтер имеет физическое устройство для печати. Только для чтения.|
|isAcceptingJobs|Boolean|Принимает ли принтер новые задания печати.|
|location|[printerLocation](printerlocation.md)|Физическое и/или организационное расположение принтера.|
|defaults|[printerDefaults](printerdefaults.md)|Параметры печати принтера по умолчанию.|
|capabilities|[printerCapabilities](printercapabilities.md)|Возможности принтера, связанного с этой обоймой принтера.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|jobs|[Коллекция printJob](printjob.md)| Список заданий, которые находятся в очереди для печати принтером.|
|shares|[Коллекция printerShare](printershare.md)| Список printerShares, связанных с принтером. В настоящее время с принтером может быть связан только один printerShare. Только для чтения. Допускается значение null.|
|соединители|[printConnector](printconnector.md)|Соединители, связанные с принтером.|
|taskTriggers|[Коллекция printTaskTrigger](printtasktrigger.md)|Список триггеров задач, связанных с принтером.|

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


