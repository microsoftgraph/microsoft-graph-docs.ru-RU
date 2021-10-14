---
title: тип ресурса printService
description: Представляет описание конкретного клиента Azure AD экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (например, обнаружения, уведомления, регистрации и IPP) и имеют одну или несколько конечных точек.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 08b5a0857a62e91f545c6678398f54c4585436be
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60355241"
---
# <a name="printservice-resource-type"></a>тип ресурса printService

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет описание конкретного клиента Azure AD экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (обнаружения, уведомлений, регистрации и IPP) и имеют одну или несколько конечных точек.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Службы списка](../api/print-list-services.md) | [коллекция printService](printservice.md) | Получите список служб универсальной печати. |
| [Получить службу](../api/printservice-get.md) | [printService](printservice.md) | Ознакомьтесь с свойствами и отношениями объекта-службы. |
| [Перечисление конечных точек](../api/printservice-list-endpoints.md) | [коллекция printServiceEndpoint](printserviceendpoint.md) | Получите список конечных точек, которые предоставляет служба. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор службы. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|endpoints|[коллекция printServiceEndpoint](printserviceendpoint.md)| Конечные точки, которые можно использовать для доступа к службе. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printService",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "endpoints": [ {"@odata.type": "microsoft.graph.printServiceEndpoint"} ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

