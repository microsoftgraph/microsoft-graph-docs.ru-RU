---
title: тип ресурса searchAlterationOptions
description: Предоставляет параметры изменения поиска для коррекции правописания.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dc17698715b4ea6e894ae13f1999e78ab361cc5e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068245"
---
# <a name="searchalterationoptions-resource-type"></a>тип ресурса searchAlterationOptions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет параметры изменения поиска для коррекции правописания.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|enableSuggestion|Логический|Указывает, включены ли предложения орфографии. Если включен, пользователь получит результаты поиска для исходного запроса поиска и предложит исправление [](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) орфографии в **свойстве queryAlterationResponse** ответа на опечатки в запросе. Необязательный.|
|enableModification|Логический|Указывает, включены ли изменения орфографии. Если включен, пользователь получит результаты поиска  для исправленного запроса, если нет результатов для исходного запроса с опечатки и получит сведения о внесении изменений орфографии в **свойство queryAlterationResponse** ответа [.](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) Необязательный.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "enableSuggestion": true,
  "enableModification": true
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
