---
title: тип ресурса printServiceEndpoint
description: Представляет URI и идентифицирует сведения для экземпляра службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7534e538c81c543671d996c7765125eafcad9d67cddbb13ad406d06edb8b9912
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178040"
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
|displayName|String|Имя отображения для конечной точки с читаемым для человека.|
|id|String|Уникальное имя, которое идентифицирует службу, которую предоставляет конечная точка. Возможные значения: `discovery` (Служба обнаружения), `notification` (Служба уведомлений), `ipp` (служба IPP) и `registration` (Служба регистрации). Только для чтения.|
|uri|String|URI, который можно использовать для доступа к службе.|


## <a name="relationships"></a>Связи
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

