---
title: тип ресурса printService
description: Представляет описание конкретного клиента Azure AD экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (например, обнаружения, уведомления, регистрации и IPP) и имеют одну или несколько конечных точек.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 6971d34f2b2e3ee023a6bb2e57d5d02ca7de3bfb54b1571d4182905e3666f9b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178054"
---
# <a name="printservice-resource-type"></a>тип ресурса printService

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

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

