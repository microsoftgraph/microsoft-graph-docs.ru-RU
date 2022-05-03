---
title: Тип ресурса printDocument
description: Представляет печатаемый документ.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 55eaea78c960596beab18682209acad9522c00d1
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176902"
---
# <a name="printdocument-resource-type"></a>Тип ресурса printDocument

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет печатаемый документ.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание сеанса отправки](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | Создайте сеанс отправки для последовательной отправки диапазонов двоичного файла **printDocument**. |
| [Скачивание двоичного файла](../api/printdocument-get-file.md) | Скачать URL-адрес | Скачайте двоичный файл, связанный с **printDocument**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор документа. Только для чтения.|
|displayName|Строка|Имя документа. Только для чтения.|
|contentType|String|Тип содержимого документа (MIME). Только для чтения.|
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


