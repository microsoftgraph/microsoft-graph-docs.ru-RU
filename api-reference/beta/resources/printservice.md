---
title: Тип ресурса printService
description: Представляет Azure AD конкретного клиента экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (например, обнаружения, уведомлений, регистрации и IPP) и имеют одну или несколько конечных точек.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: df904704f6efb9d069832a6b9767ab1314e261ee
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176761"
---
# <a name="printservice-resource-type"></a>Тип ресурса printService

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Azure AD конкретного клиента экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (обнаружение, уведомления, регистрация и IPP) и имеют одну или несколько конечных точек.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление служб](../api/print-list-services.md) | [Коллекция printService](printservice.md) | Получение списка служб универсальной печати. |
| [Получение службы](../api/printservice-get.md) | [printService](printservice.md) | Чтение свойств и связей объекта службы. |
| [Перечисление конечных точек](../api/printservice-list-endpoints.md) | [Коллекция printServiceEndpoint](printserviceendpoint.md) | Получение списка конечных точек, которые предоставляет служба. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор службы. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|endpoints|[Коллекция printServiceEndpoint](printserviceendpoint.md)| Конечные точки, которые можно использовать для доступа к службе. Только для чтения. Допускается значение null.|

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

