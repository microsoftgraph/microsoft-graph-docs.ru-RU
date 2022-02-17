---
title: тип ресурса searchAlteration
description: Предоставляет сведения об изменениях поиска для исправления орфографии.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 9c89193a3d57f8dcb701e57e98160ee69b8a8a91
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878704"
---
# <a name="searchalteration-resource-type"></a>тип ресурса searchAlteration

Пространство имен: microsoft.graph

Предоставляет сведения об изменениях поиска для исправления орфографии.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|alteredHighlightedQueryString|Строка| Определяет измененную выделенную строку запроса с помощью коррекции орфографии. Аннотация вокруг исправленного сегмента: `\ue000, \ue001`.|
|alteredQueryString|String| Определяет измененную строку запроса с помощью коррекции орфографии.|
|alteredQueryTokens|[измененная коллекцияQueryToken](alteredquerytoken.md)| Представляет измененные сегменты, связанные с исходным запросом пользователя.|

## <a name="json-representation"></a>Представление JSON

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
  "alteredHighlightedQueryString": "String",
  "alteredQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```
