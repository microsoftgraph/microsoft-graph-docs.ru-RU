---
title: Тип ресурса print
description: При подписке на универсальную печать функция печати позволяет управлять принтерами и обнаруживать точки printServiceEndpoints, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0604044824d153c9e6d39586c2ca58ee9ca893ea
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292261"
---
# <a name="print-resource-type"></a>Тип ресурса print

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При подписке на универсальную печать функция печати позволяет управлять принтерами и обнаруживать точки [printServiceEndpoints,](printserviceendpoint.md) которые можно использовать для управления принтерами и заданиями печати в универсальной печати.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление соединителей](../api/print-list-connectors.md) | [Коллекция printConnector](printconnector.md) | Получите список соединители печати. |
| [Перечисление принтеров](../api/print-list-printers.md) | [коллекция принтеров](printer.md) | Получите список принтеров. |
| [Перечисление общих ресурсов](../api/print-list-shares.md) | [Коллекция printerShare](printershare.md) | Получите список обетов принтеров. |
| [Список служб](../api/print-list-services.md) | [Коллекция printService](printservice.md) | Получите список служб. |
| [Создание printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | Создание новой обоймы принтера путем публикации в **коллекции.** |
| [Создание принтера](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создайте (зарегистрируйте) новый принтер с помощью универсальной печати. |
| [Обновление параметров](../api/print-update-settings.md) |  [printSettings](printsettings.md) | Обновляет параметры службы универсальной печати на всем клиенте. |
| [Перечисление taskDefinitions](../api/print-list-taskdefinitions.md) | [Коллекция printTaskDefinition](printtaskdefinition.md) | Получите список printTaskDefinitions на всем клиенте, созданный в универсальной печати. |
| [Создание taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создайте новый printTaskDefinition. |
| [Обновление taskDefinition](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Обновление printTaskDefinition. |
| [Удаление taskDefinition](../api/print-delete-taskdefinition.md) | Нет | Удаление printTaskDefinition. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|параметры|[printSettings](printsettings.md)|Параметры универсальной печати на всем клиенте.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|services|[Коллекция printService](printservice.md)|Список доступных конечных точек службы универсальной печати.|
|printers|[коллекция принтеров](printer.md)|Список принтеров, зарегистрированных в клиенте.|
|shares|[Коллекция printerShare](printershare.md)|Список акций принтера, зарегистрированных в клиенте.|
|соединители|[Коллекция printConnector](printconnector.md)|Список доступных соединители печати.|

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
  ]
}-->


