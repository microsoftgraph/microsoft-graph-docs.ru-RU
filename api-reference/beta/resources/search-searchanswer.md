---
title: тип ресурса searchAnswer
description: Ответ поиска — это базовый тип для других ответов поиска.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 06fa9cfe754af55d4ee19640a9d75c00b7dbca2f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339521"
---
# <a name="searchanswer-resource-type"></a>тип ресурса searchAnswer

Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ответ поиска — это базовый тип для других ответов поиска, таких как аббревиатура [,](../resources/search-acronym.md) закладки [и](../resources/search-bookmark.md) [ресурсы QnA](../resources/search-qna.md) . Включает свойства, применимые к другим объектам ответов поиска.


Наследуется [от сущности](../resources/entity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор (GUID) для ответа на запрос. Наследуется [от сущности](../resources/entity.md).|
|displayName|Строка|Имя ответа поиска, отображаемая в результатах поиска.|
|description|String|Описание ответов поиска, показанное на странице результатов поиска.|
|webUrl|String|Ссылка URL-адрес ответа поиска. Когда пользователи щелкают этот ответ поиска в результатах поиска, они перейдут на этот URL-адрес.|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/identityset.md)|Сведения о пользователе, который создал или в последний раз изменил ответ на поиск. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время создания или редактирования ответа на поиск. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.search.searchAnswer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.searchAnswer",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

