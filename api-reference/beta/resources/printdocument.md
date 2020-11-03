---
title: Тип ресурса printDocument
description: Представляет документ, который печатается.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c0bc886b618e061bee51ad82d7032737015f58ab
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849216"
---
# <a name="printdocument-resource-type"></a>Тип ресурса printDocument

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет документ, который печатается.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание сеанса отправки](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | Создайте сеанс отправки для последовательной отправки диапазонов двоичного файла **printDocument**. |
| [Скачать двоичный файл](../api/printdocument-get-file.md) | URL-адрес скачивания | Скачайте двоичный файл, связанный с классом **printDocument**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор документа. Только для чтения.|
|displayName|String|Имя документа. Только для чтения.|
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


