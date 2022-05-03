---
title: Тип ресурса print
description: При использовании подписки на универсальную печать функция "Печать" позволяет управлять принтерами и обнаруживать точки printServiceEndpoint, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b95c2d31b615fcf649dca8e88a4bff51b3376df4
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176697"
---
# <a name="print-resource-type"></a>Тип ресурса print

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

При использовании подписки на универсальную печать функция "Печать" позволяет управлять принтерами и обнаруживать точки [printServiceEndpoint,](printserviceendpoint.md) которые можно использовать для управления принтерами и заданиями печати в универсальной печати.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление соединителей](../api/print-list-connectors.md) | [Коллекция printConnector](printconnector.md) | Получение списка соединителей печати. |
| [Перечисление принтеров](../api/print-list-printers.md) | [коллекция принтеров](printer.md) | Получение списка принтеров. |
| [Перечисление общих ресурсов](../api/print-list-shares.md) | [Коллекция printerShare](printershare.md) | Получение списка общих папок принтера. |
| [Перечисление служб](../api/print-list-services.md) | [Коллекция printService](printservice.md) | Получение списка служб. |
| [Создание printerShare](../api/print-post-shares.md) | [printerShare](printershare.md) | Создайте общую папку принтера, выполнив публикацию в **коллекции общих** папок. |
| [Создание принтера](../api/printer-create.md) | [printerCreateOperation](printerCreateOperation.md) | Создайте (зарегистрируйте) новый принтер с универсальной печатью. |
| [Обновление параметров](../api/print-update-settings.md) |  [printSettings](printsettings.md) | Обновляет параметры на уровне клиента для службы универсальной печати. |
| [Перечисление taskDefinitions](../api/print-list-taskdefinitions.md) | [Коллекция printTaskDefinition](printtaskdefinition.md) | Получение списка printTaskDefinitions на уровне клиента, созданных в рамках универсальной печати. |
| [Создание taskDefinition](../api/print-post-taskdefinitions.md) | [printTaskDefinition](printtaskdefinition.md) | Создайте printTaskDefinition. |
| [Обновление taskDefinition](../api/print-update-taskdefinition.md) | [printTaskDefinition](printtaskdefinition.md) | Обновление printTaskDefinition. |
| [Удаление taskDefinition](../api/print-delete-taskdefinition.md) | Нет | Удалите printTaskDefinition. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|settings|[printSettings](printsettings.md)|Параметры универсальной печати на уровне клиента.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Услуги|[Коллекция printService](printservice.md)|Список доступных конечных точек службы универсальной печати.|
|Принтеры|[коллекция принтеров](printer.md)|Список принтеров, зарегистрированных в клиенте.|
|shares|[Коллекция printerShare](printershare.md)|Список общих папок принтера, зарегистрированных в клиенте.|
|connectors|[Коллекция printConnector](printconnector.md)|Список доступных соединителей печати.|

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


