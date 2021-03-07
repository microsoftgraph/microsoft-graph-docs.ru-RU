---
title: тип ресурса printServiceEndpoint
description: Представляет URI и идентифицирует сведения для экземпляра службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0dd339d433be593e6982b6c38818635830a2d471
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517458"
---
# <a name="printserviceendpoint-resource-type"></a>тип ресурса printServiceEndpoint

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет URI и идентифицирует сведения для экземпляра службы печати.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Получение конечной точки](../api/printserviceendpoint-get.md) | [printServiceEndpoint](printserviceendpoint.md) | Ознакомьтесь с свойствами и отношениями конечного объекта. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Имя отображения для конечной точки с читаемым для человека.|
|id|Строка|Уникальное имя, которое идентифицирует службу, которую предоставляет конечная точка. Возможные значения: `discovery` (Служба обнаружения), `notification` (Служба уведомлений), `ipp` (служба IPP) и `registration` (Служба регистрации). Только для чтения.|
|uri|Строка|URI, который можно использовать для доступа к службе.|


## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "String (identifier)",
  "displayName": "String",
  "uri": "String"
}
```

