---
title: тип ресурса searchAlterationOptions
description: Предоставляет параметры изменения поиска для коррекции правописания.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1692cf40700c9af40b4ecab77b32210291e60f78
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878700"
---
# <a name="searchalterationoptions-resource-type"></a>тип ресурса searchAlterationOptions

Пространство имен: microsoft.graph

Предоставляет параметры изменения поиска для коррекции правописания.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|enableModification|Логический|Указывает, включены ли изменения орфографии. Если включен, пользователь получит результаты поиска для исправленного запроса, если результатов для исходного запроса с помощью опечаток не будет. Ответ [также](/graph/api/resources/searchresponse) будет включать сведения об изменении орфографии в **свойстве queryAlterationResponse** . Необязательное свойство.|
|enableSuggestion|Логический|Указывает, включены ли предложения орфографии. Если включено, пользователь получит результаты поиска для исходного запроса поиска и предложения по исправлению орфографии в свойстве **queryAlterationResponse** ответа на опечатки в запросе.[](/graph/api/resources/searchresponse) Необязательное свойство.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlterationOptions",
  "baseType": null
}-->

```json
{
  "enableModification": "Boolean",
  "enableSuggestion": "Boolean"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchAlterationOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
