---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 102cf81f0770f02b1206bff1fa927121696047c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727978"
---
# <a name="printdocument-resource-type"></a>Тип ресурса printDocument

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет документ, который печатается.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание сеанса отправки](../api/printdocument-get-file.md) | [uploadSession](uploadsession.md) | Создайте сеанс отправки для последовательной отправки диапазонов двоичного файла **printDocument**. |
| [Скачать двоичный файл](../api/printdocument-get-file.md) | URL-адрес скачивания | Скачайте двоичный файл, связанный с классом **printDocument**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор документа. Только для чтения.|
|displayName|Строка|Имя документа. Только для чтения.|
|contentType|String|Тип контента документа (MIME). Только для чтения.|
|size|Int64|Размер документа в байтах. Только для чтения.|

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
  "displayName": "String",
  "contentType": "String",
  "size": 12345
}

```


