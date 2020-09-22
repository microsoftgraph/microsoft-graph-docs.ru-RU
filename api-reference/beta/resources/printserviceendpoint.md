---
title: Тип ресурса Принтсервицеендпоинт
description: Представляет URI и идентификационные данные для экземпляра службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8b9289807778c1a44940d8e8eb0d9163ed12f006
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985862"
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
|displayName|String|Понятное для пользователя отображаемое имя для конечной точки.|
|name|String|Уникальное имя, идентифицирующее службу, которую предоставляет конечная точка. Возможные значения: `discovery` (служба обнаружения), `notification` (служба уведомлений), `ipp` (Служба протокола IPP) и `registration` (служба регистрации). Только для чтения.|
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

