---
title: Тип ресурса Сеарчрекуест
description: Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fe3117eae0e514bea979281220da12820574cb4a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520901"
---
# <a name="searchrequest-resource-type"></a>Тип ресурса Сеарчрекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запрос поиска, отправляемый конечной точке запроса. Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрос полей и фактический поисковый запрос.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|stored_fields|Коллекция объектов string |Содержит поля, возвращаемые для объекта еарч _so урцес. Обратите внимание, что этот параметр применяется`externalItem` , только если в отклике указан тип EntityType =.|
|contentSources|Коллекция объектов string|Содержит подключение, которое необходимо задать. <br>В соответствии со следующим `/external/connections/connectionid` форматом `connectionid` : где Коннектионид был определен в администрировании соединителей <br> Note contentSource применяется только в том случае,`externalItem`если EntityType =. |
|enableTopResults|Boolean|Это запускает гибридную сортировку для сообщений: первые 3 сообщения наиболее актуальны<br> Это относится только к типу entityType =`message`.|
|entityTypes|Коллекция `entityType`| Возможные значения: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.|
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
