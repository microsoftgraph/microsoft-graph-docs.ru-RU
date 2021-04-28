---
title: тип ресурса searchAlteration
description: Предоставляет сведения об изменениях поиска для исправления орфографии.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5caab3a3fbd8f8487e6893c5f5f530cc8471bb80
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068242"
---
# <a name="searchalteration-resource-type"></a>тип ресурса searchAlteration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения об изменениях поиска для исправления орфографии.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|alteredQueryString|String| Определяет измененную строку запроса с помощью коррекции орфографии.|
|alteredHighlightedQueryString|String| Определяет измененную выделенную строку запроса с помощью коррекции орфографии. Аннотация вокруг исправленного сегмента (\ue000, \ue001)|
|alteredQueryTokens|[измененная коллекцияQueryToken](alteredquerytoken.md)| Представляет измененные сегменты в отношении исходного запроса.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlteration",
  "baseType": null
}-->

```json
{
  "alteredQueryString": "String",
  "alteredHighlightedQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```