---
title: тип ресурса printDocument
description: Представляет печатаемый документ.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4e2c8359b49e2154e3f107c97edf93fc64bd394837d5cf8ca8b1daa14446b857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169370"
---
# <a name="printdocument-resource-type"></a>тип ресурса printDocument

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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