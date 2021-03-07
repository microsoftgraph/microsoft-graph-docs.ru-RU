---
title: тип ресурса printService
description: Представляет описание конкретного клиента Azure AD экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (например, обнаружения, уведомления, регистрации и IPP) и имеют одну или несколько конечных точек.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 986749028a75f98157ff73138396a4ad56672fc8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517463"
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
|id|Строка|Идентификатор службы. Только для чтения.|

## <a name="relationships"></a>Отношения
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

