---
title: Тип ресурса printerCreateOperation
description: Представляет долго выполняющуюся операцию регистрации принтера. Является производным от printOperation.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 716c23603dd811ddad61dd604c9961d1df3f5297
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176533"
---
# <a name="printercreateoperation-resource-type"></a>Тип ресурса printerCreateOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет долго выполняющуюся операцию регистрации принтера. Является производным [от printOperation](printoperation.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Операция Get](../api/printoperation-get.md) | [printOperation](printoperation.md) | Получение длительной операции в клиенте текущего пользователя или приложения. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор операции. Только для чтения.|
|status|[printOperationStatus](printoperationstatus.md)|Состояние операции регистрации. Содержит ход выполнения операции и ее успешное выполнение. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset при создании операции. Только для чтения.|
|certificate|String|Подписанный сертификат, созданный во время регистрации. Только для чтения.|
|Принтера|[printer](printer.md)|Созданная сущность принтера. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z",
    "certificate": "",
    "printer": {"@odata.type": "microsoft.graph.printer"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCreateOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

