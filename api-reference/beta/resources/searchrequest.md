---
title: Тип ресурса Сеарчрекуест
description: Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fac759f190f193fb2fe37e769feedc1164fc3f95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973742"
---
# <a name="searchrequest-resource-type"></a>Тип ресурса Сеарчрекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|stored_fields|Коллекция String |Содержит поля, возвращаемые для объекта еарч _so урцес. Обратите внимание, что этот параметр применяется, только если `externalItem` в отклике указан тип EntityType =.|
|contentSources|Коллекция String|Содержит подключение, которое необходимо задать. <br>В соответствии со следующим форматом: `/external/connections/connectionid` где `connectionid` коннектионид был определен в администрировании соединителей <br> Note contentSource применяется только в том случае, если entityType = `externalItem` . |
|enableTopResults|Boolean|Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее актуальны<br> Это относится только к типу entityType = `message` .|
|entityTypes|Коллекция `entityType`| Возможные значения: `event`, `message`, `driveItem`, `externalItem`.|
|from|Int32|Задает смещение результатов поиска. Смещение 0 возвращает самый первый результат.|
|Запрос|[searchQuery](searchquery.md)|Содержит термины запроса.|
|size|Int32|Размер извлекаемой страницы.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "stored_fields": ["String"],
  "contentSources": ["String"],
  "entityTypes": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "enableTopResults": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


