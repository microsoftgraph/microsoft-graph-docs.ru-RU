---
title: тип ресурса printOperation
description: Представляет собой долгосрочную операцию универсальной печати. Базовый класс для типов операций, таких как printerCreateOperation.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 55bf24e75f79a66d9691b14ebac1073c43f15a4e
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60942508"
---
# <a name="printoperation-resource-type"></a>тип ресурса printOperation

Пространство имен: microsoft.graph

Представляет собой долгосрочную операцию универсальной печати. Базовый класс для типов операций, таких как [printerCreateOperation.](printercreateoperation.md)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Получить операцию](../api/printoperation-get.md) | [printOperation](printoperation.md) | Извлечение длительной операции в текущем пользователе или клиенте приложения. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор операции. Только для чтения.|
|status|[printOperationStatus](printoperationstatus.md)|Состояние операции. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset, когда была создана операция. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)"
}
```

