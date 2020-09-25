---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfe1badffdd675c68678e1f8463d09aee2af1217
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273685"
---
# <a name="printdocument-resource-type"></a>Тип ресурса printDocument

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет документ, который печатается.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [уплоаддата](../api/printdocument-uploaddata.md) | Нет | Отправьте один двоичный сегмент **printDocument**. |
| [Скачать двоичный файл](../api/printdocument-get-file.md) | URL-адрес скачивания | Скачайте двоичный файл, связанный с классом **printDocument**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор документа. Только для чтения.|
|displayName|String|Имя документа. Только для чтения.|
|contentType|String|Тип контента документа (MIME). Только для чтения.|
|size|Int64|Размер документа в байтах. Только для чтения.|
|configuration|[принтердокументконфигуратион](printerdocumentconfiguration.md) |Группа параметров, которые принтер должен использовать для печати документа. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "mimeType": "String",
  "sizeInBytes": 12345,
  "documentConfiguration": {
    "pageRanges": [ {"@odata.type": "microsoft.graph.printPageRange"} ],
    "printQuality": "String",
    "printResolutionInDpi": 123456,
    "feedDirection": "String",
    "orientation": "String",
    "duplexConfiguration": "String",
    "copies": 123456,
    "colorConfiguration": "String",
  }
}

```


