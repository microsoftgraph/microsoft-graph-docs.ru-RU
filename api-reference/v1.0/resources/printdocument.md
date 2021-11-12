---
title: тип ресурса printDocument
description: Представляет печатаемый документ.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 86af8835c4452f379aadd4bfd23e87a9029045d4
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945007"
---
# <a name="printdocument-resource-type"></a>тип ресурса printDocument

Пространство имен: microsoft.graph

Представляет печатаемый документ.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Создание сеанса загрузки](../api/printdocument-createuploadsession.md) | [uploadSession](uploadsession.md) | Создание сеанса загрузки в итеративный диапазоны загрузки двоичного файла **printDocument**. |
| [Скачивание двоичного файла](../api/printdocument-get-file.md) | Скачать URL-адрес | Скачайте двоичный файл, связанный с **печатьюDocument**. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор документа. Только для чтения.|
|displayName|String|Имя документа. Только для чтения.|
|contentType|String|Тип контента документа (MIME). Только для чтения.|
|size|Int64|Размер документа в bytes. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printDocument",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": "Integer"
}
```
