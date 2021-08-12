---
title: тип ресурса printOperation
description: Представляет собой долгосрочную операцию универсальной печати. Базовый класс для типов операций, таких как printerCreateOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0630d05e30d415ad60f4dd7ea4e7f729506e41b2cc20bded955e1593a6f56161
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138460"
---
# <a name="printoperation-resource-type"></a>тип ресурса printOperation

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

