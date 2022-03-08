---
title: тип ресурса answerKeyword
description: Ключевые слова ответов позволяют пользователям определять слова и фразы, которые будут вызывать ответ на административный поиск, появляться в результатах поиска.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b63a3a286528c7b1e7a1f87759cf7635499bde01
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339534"
---
# <a name="answerkeyword-resource-type"></a>тип ресурса answerKeyword

Пространство имен: microsoft.graph.search

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ключевое слово ответа используется для настройки слов и фраз, которые будут вызывать ответ на административный поиск, появляться в результатах поиска.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|keywords|Коллекция String|Набор ключевых слов, используемых для запуска ответа на поиск.|
|matchSimilarKeywords|Boolean|Если `true`, указывает, что термин поиска содержит похожие слова на ключевые слова, которые должны вызвать ответ на поиск.|
|reservedKeywords|Коллекция строк|Запускаются уникальные ключевые слова, которые гарантируют ответ на поиск.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.search.answerKeyword"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.search.answerKeyword",
  "keywords": [
    "String"
  ],
  "reservedKeywords": [
    "String"
  ],
  "matchSimilarKeywords": "Boolean"
}
```

