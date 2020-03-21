---
title: Тип ресурса Принтсервицеендпоинт
description: Представляет URI и идентификационные данные для экземпляра службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7f28245c22916575d505b3e9f8db65070cbbbf5e
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896062"
---
# <a name="printserviceendpoint-resource-type"></a>Тип ресурса Принтсервицеендпоинт

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет URI и идентификационные данные для экземпляра службы печати.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение конечной точки](../api/printserviceendpoint-get.md) | [принтсервицеендпоинт](printserviceendpoint.md) | Считывание свойств и связей объекта Endpoint. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Понятное для пользователя отображаемое имя для конечной точки.|
|name|String|Уникальное имя, идентифицирующее службу, которую предоставляет конечная точка. `discovery` Возможные значения: (служба обнаружения) `notification` , (служба уведомлений), `ipp` (Служба протокола IPP) и `registration` (служба регистрации). Только для чтения.|
|URI|String|Универсальный код ресурса (URI), который можно использовать для доступа к службе.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}-->

```json
{
  "displayName": "String",
  "name": "String (identifier)",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printServiceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->