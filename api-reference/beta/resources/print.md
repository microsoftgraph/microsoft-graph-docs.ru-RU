---
title: Тип ресурса Print
description: С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать Принтсервицеендпоинтс, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 551fa42736d6fa275a8f998274a6fccf55ac00b7
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006977"
---
# <a name="print-resource-type"></a>Тип ресурса Print

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать [принтсервицеендпоинтс](printserviceendpoint.md) , которые можно использовать для управления принтерами и заданиями печати в универсальной печати.

## <a name="methods"></a>Методы
| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список соединителей](../api/print-list-connectors.md) | Коллекция [принтконнектор](printconnector.md) | Получение списка соединителей печати. |
| [Список принтеров](../api/print-list-printers.md) | Коллекция [принтеров](printer.md) | Получение списка принтеров. |
| [Список общих папок](../api/print-list-shares.md) | Коллекция [принтершаре](printershare.md) | Получение списка общих принтеров. |
| [Список служб](../api/print-list-services.md) | Коллекция [принтсервице](printservice.md) | Получение списка служб. |
| [Создание Принтершаре](../api/print-post-shares.md) | [принтершаре](printershare.md) | Создайте новый общий ресурс для принтера, отправив его в коллекцию **shares** . |
| [Создание принтера](../api/printer-create.md) | [принтеркреатеоператион](printerCreateOperation.md) | Создание (регистрация) нового принтера с универсальной печатью. |
| [Обновление параметров](../api/print-update-settings.md) |  [принтсеттингс](printsettings.md) | Обновляет параметры на уровне клиента для универсальной службы печати. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|settings|[принтсеттингс](printsettings.md)|Параметры на уровне клиента для универсальной службы печати.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|служб|Коллекция [принтсервице](printservice.md)|Список доступных конечных точек универсальной службы печати.|
|типографи|Коллекция [принтеров](printer.md)|Список принтеров, зарегистрированных в клиенте.|
|shares|Коллекция [принтершаре](printershare.md)|Список общих принтеров, зарегистрированных в клиенте.|
|аудиовыход|Коллекция [принтконнектор](printconnector.md)|Список доступных соединителей печати.|

## <a name="json-representation"></a>Представление в формате JSON

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
