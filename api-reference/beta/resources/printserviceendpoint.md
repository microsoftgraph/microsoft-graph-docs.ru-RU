---
title: Тип ресурса printServiceEndpoint
description: Представляет универсальный код ресурса (URI) и идентифицирует сведения для экземпляра службы печати.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3c5d9085614b4c4ad99aa43cb8281a3123eb3741
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176751"
---
# <a name="printserviceendpoint-resource-type"></a>Тип ресурса printServiceEndpoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет универсальный код ресурса (URI) и идентифицирует сведения для экземпляра службы печати.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение конечной точки](../api/printserviceendpoint-get.md) | [printServiceEndpoint](printserviceendpoint.md) | Чтение свойств и связей объекта конечной точки. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Понятное для человека отображаемое имя конечной точки.|
|name|String|Уникальное имя, определяющее службу, которую предоставляет конечная точка. Возможные значения: `discovery` (служба обнаружения), `notification` (служба уведомлений), `ipp` (служба IPP) и `registration` (служба регистрации). Только для чтения.|
|Uri|Строка|Универсальный код ресурса (URI), который можно использовать для доступа к службе.|

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

