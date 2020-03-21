---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a44cac259e9be653ca0e7b21c81b6c72224268b1
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896017"
---
# <a name="printershare-resource-type"></a>Тип ресурса Принтершаре

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Принтершарес](../api/print-list-printershares.md) | Коллекция [принтершаре](printershare.md) | Получение списка общих принтеров в клиенте. |
| [Получение Принтершаре](../api/printershare-get.md) | [принтершаре](printershare.md) | Чтение свойств и связей объекта Принтершаре. |
| [обновление](../api/printershare-update.md). | [принтершаре](printershare.md) | Обновление объекта Принтершаре. |
| [удаление](../api/printershare-delete.md); | Нет | Отменяет общий доступ к принтеру. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Идентификатор Принтершаре. Только для чтения.|
|name|String|Имя общего принтера, который должен отображаться клиентами печати.|
|createdDateTime|DateTimeOffset|Значение DateTimeOffset при создании общего ресурса принтера. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|Printer|[Printer](printer.md)|Принтер, с которым связан этот общий принтер. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->