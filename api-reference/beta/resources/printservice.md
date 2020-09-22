---
title: Тип ресурса Принтсервице
description: Представляет специфическое для клиента Azure AD описание экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (например, обнаружение, уведомления, регистрация и протокол IPP) и имеют одну или несколько конечных точек.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 00ba50369f2396250df632c13ed3945e8c9d40d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052545"
---
# <a name="printservice-resource-type"></a>Тип ресурса Принтсервице

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет специфическое для клиента Azure AD описание экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (обнаружение, уведомления, регистрация и протокол IPP) и имеют одну или несколько конечных точек.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список служб](../api/print-list-services.md) | Коллекция [принтсервице](printservice.md) | Получение списка универсальных служб печати. |
| [Получение службы](../api/printservice-get.md) | [принтсервице](printservice.md) | Считывание свойств и связей объекта Service. |
| [Перечисление конечных точек](../api/printservice-list-endpoints.md) | Коллекция [принтсервицеендпоинт](printserviceendpoint.md) | Получение списка конечных точек, предоставляемых службой. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор службы. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|endpoints|Коллекция [принтсервицеендпоинт](printserviceendpoint.md)| Конечные точки, которые можно использовать для доступа к службе. Только для чтения. Допускается значение null.|

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

