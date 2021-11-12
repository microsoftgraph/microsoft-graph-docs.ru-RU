---
title: тип ресурса printService
description: Представляет описание конкретного клиента Azure AD экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (например, обнаружения, уведомления, регистрации и IPP) и имеют одну или несколько конечных точек.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7319ee78846f98f0d41faab9deecff6bc2b1830b
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936959"
---
# <a name="printservice-resource-type"></a>тип ресурса printService

Пространство имен: microsoft.graph

Представляет описание конкретного клиента Azure AD экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (обнаружения, уведомлений, регистрации и IPP) и имеют одну или несколько конечных точек.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Службы списка](../api/print-list-services.md) | [коллекция printService](printservice.md) | Получите список служб универсальной печати. |
| [Получить службу](../api/printservice-get.md) | [printService](printservice.md) | Ознакомьтесь с свойствами и отношениями объекта-службы. |
| [Перечисление конечных точек](../api/printservice-list-endpoints.md) | [коллекция printServiceEndpoint](printserviceendpoint.md) | Получите список конечных точек, которые предоставляет служба. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор службы. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|endpoints|[коллекция printServiceEndpoint](printserviceendpoint.md)| Конечные точки, которые можно использовать для доступа к службе. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printService",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printService",
  "id": "String (identifier)"
}
```

