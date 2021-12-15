---
title: тип ресурса bookingQuestionAnswer
description: Содержит настраиваемый вопрос, ответ клиента на настраиваемый вопрос и свойства настраиваемого вопроса на момент создания встречи.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 9c8d45ebea2045c125f6a7d466e9bed14ff8ec1d
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525666"
---
# <a name="bookingquestionanswer-resource-type"></a>тип ресурса bookingQuestionAnswer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит настраиваемый вопрос, ответ клиента на настраиваемый вопрос и свойства настраиваемого вопроса на момент создания встречи.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ответ|Строка|Ответ, данный пользователем в случае **ответаInputType** `text` . |
|answerInputType|answerInputType|Ожидаемый тип ответа. Допустимые значения: `text`, `radioButton`, `unknownFutureValue`.|
|answerOptions|Коллекция строк|В случае, если answerInputType — это radioButton, он будет состоять из списка возможных значений ответов. |
|isRequired|Boolean| Указывает, обязательно ли отвечать на настраиваемый вопрос. |
|вопрос|Строка|Вопрос. |
|questionId|Строка|ID настраиваемого вопроса. |
|selectedOptions|Коллекция строк|Ответы, выбранные пользователем. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingQuestionAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingQuestionAnswer",
  "questionId": "String",
  "question": "String",
  "answerInputType": {"@odata.type": "microsoft.graph.answerInputType"},
  "answerOptions": [
    "String"
  ],
  "isRequired": "Boolean",
  "answer": "String",
  "selectedOptions": [
    "String"
  ]
}
```

