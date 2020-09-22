---
title: Тип ресурса Експиратионпаттерн
description: Шаблон истечения срока действия в расписании запросов можно включить в запрос на назначение пакета Access и он присутствует в назначении пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f9200d336ae69ae02c45ab1d6fc3d9df86691ebc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026980"
---
# <a name="expirationpattern-resource-type"></a>Тип ресурса Експиратионпаттерн

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении обслуживанием в Azure AD](entitlementmanagement-root.md)запрос на назначение пакета Access создается пользователем, желающим получить назначение пакета Access. Этот запрос может включать расписание, когда пользователь хочет назначить назначение.  Назначение пакета Access, полученное в результате такого запроса, также имеет расписание.  Поле истечения срока действия [рекуестсчедуле](requestschedule.md) указывает, когда истечет срок действия назначения пакета Access.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|duration|Длительность|Предполагаемая длительность доступа запрашивающего. Если это указано в запросе, endDateTime не должно присутствовать.|
|type|експиратионпаттернтипе|Нужный тип шаблона срока действия запрашивающего.|

### <a name="expirationpatterntype-values"></a>значения Експиратионпаттернтипе

| Элемент | Значение| Описание |
|:---------------|:--------|:----------|
|нотспеЦифиед|нуль|Расписание истечения срока действия не указано.|
|неограниченный срок действия|1 |Запрашивающая сторона не предоставила срок действия доступа.|
|афтердатетиме|2 |Срок действия доступа через указанную дату и время истечет.|
|афтердуратион|4|Срок действия доступа истекает через указанное время относительно предоставления доступа.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern",
  "baseType": ""
}-->

```json
{
    "endDateTime": "2020-09-10T23:06:53.307Z",
    "type": "afterDateTime"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expirationPattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


