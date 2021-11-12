---
title: тип ресурса printerCreateOperation
description: Представляет собой операцию длительной регистрации принтера. Производный от printOperation.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c17b30b8644206d9815044bebda563d530af8a94
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944293"
---
# <a name="printercreateoperation-resource-type"></a>тип ресурса printerCreateOperation

Пространство имен: microsoft.graph

Представляет собой операцию длительной регистрации принтера. Производные от [printOperation](printoperation.md).

Наследует [от printOperation](printoperation.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Получить операцию](../api/printoperation-get.md) | [printOperation](printoperation.md) | Извлечение длительной операции в текущем пользователе или клиенте приложения. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор операции. Только для чтения.|
|status|[printOperationStatus](printoperationstatus.md)|Состояние операции регистрации. Содержит ход операции и ее успешное завершения. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда была создана операция. Только для чтения.|
|certificate|String|Подписанный сертификат, созданный в процессе регистрации. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|printer|[printer](printer.md)|Созданный объект принтера. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "baseType": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCreateOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)",
  "certificate": "String"
}
```

