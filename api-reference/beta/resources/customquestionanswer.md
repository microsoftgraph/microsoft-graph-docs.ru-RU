---
title: тип ресурса customQuestionAnswer
description: Представляет ответ регистратора на настраиваемый вопрос о регистрации.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.date: 09/30/2021
doc_type: resourcePageType
ms.openlocfilehash: 4bed8b0c706f7ed1391465534213e849a9f0effe
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369539"
---
# <a name="customquestionanswer-resource-type"></a>тип ресурса customQuestionAnswer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ответ регистратора на [](meetingregistrationquestion.md) пользовательский вопрос регистрации, связанный с [собраниемРегистрация.](meetingregistration.md)

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| displayName | String | Отображение имени настраиваемого вопроса регистрации. Только для чтения. |
| questionId | String | ID настраиваемый вопрос регистрации. Только для чтения.|
| value | String | Ответ на настраиваемый вопрос регистрации. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customQuestionAnswer"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "value": "String"
}
```
