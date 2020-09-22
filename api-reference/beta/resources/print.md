---
title: Тип ресурса Print
description: С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать Принтсервицеендпоинтс, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 309b7c8e62b94703bb00e21fb8c8ed2a2e917efe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985890"
---
# <a name="print-resource-type"></a>Тип ресурса Print

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать [принтсервицеендпоинтс](printserviceendpoint.md) , которые можно использовать для управления принтерами и заданиями печати в универсальной печати.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление соединителей](../api/print-list-connectors.md) | Коллекция [принтконнектор](printconnector.md) | Получение списка соединителей печати. |
| [Перечисление принтеров](../api/print-list-printers.md) | Коллекция [принтеров](printer.md) | Получение списка принтеров. |
| [Перечисление общих ресурсов](../api/print-list-shares.md) | Коллекция [принтершаре](printershare.md) | Получение списка общих принтеров. |
| [Список служб](../api/print-list-services.md) | Коллекция [принтсервице](printservice.md) | Получение списка служб. |
| [Создание printerShare](../api/print-post-shares.md) | [принтершаре](printershare.md) | Создайте новый общий ресурс для принтера, отправив его в коллекцию **shares** . |
| [Создание принтера](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создание (регистрация) нового принтера с универсальной печатью. |
| [Обновление параметров](../api/print-update-settings.md) |  [принтсеттингс](printsettings.md) | Обновляет параметры на уровне клиента для универсальной службы печати. |
| [Перечисление taskDefinitions](../api/print-list-taskdefinitions.md) | Коллекция [принттаскдефинитион](printtaskdefinition.md) | Получение общего для клиента списка Принттаскдефинитионс, созданного в универсальной печати. |
| [Создание taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создание нового Принттаскдефинитион. |
| [Обновление taskDefinition](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Обновление Принттаскдефинитион. |
| [Удаление taskDefinition](../api/print-delete-taskdefinition.md) | Нет | Удаление объекта Принттаскдефинитион. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|параметры|[принтсеттингс](printsettings.md)|Параметры на уровне клиента для универсальной службы печати.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|служб|Коллекция [принтсервице](printservice.md)|Список доступных конечных точек универсальной службы печати.|
|типографи|Коллекция [принтеров](printer.md)|Список принтеров, зарегистрированных в клиенте.|
|shares|Коллекция [принтершаре](printershare.md)|Список общих принтеров, зарегистрированных в клиенте.|
|аудиовыход|Коллекция [принтконнектор](printconnector.md)|Список доступных соединителей печати.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.print",
  "keyProperty": "settings"
}-->

```json
{
  "settings": {"@odata.type": "microsoft.graph.printSettings"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "print resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource print has documented navigation properties, but we thought it was a complex type!",
    "Resource print has documented navigation properties, but we thought it was a complex type!"
}-->


