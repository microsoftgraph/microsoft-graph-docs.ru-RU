---
title: тип ресурса printerCreateOperation
description: Представляет собой операцию длительной регистрации принтера. Производный от printOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 91a1d70afccf94abe1c611e696bc4349a59964e1dbb176cce0ddb8aa32dc287a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169356"
---
# <a name="printercreateoperation-resource-type"></a>тип ресурса printerCreateOperation

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

