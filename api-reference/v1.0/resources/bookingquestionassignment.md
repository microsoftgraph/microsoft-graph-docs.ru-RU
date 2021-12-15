---
title: тип ресурса bookingQuestionAssignment
description: Содержит набор пользовательских вопросов, связанных с определенной службой.
ms.localizationpriority: medium
author: razortbone
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: dca8d753b2f2787be2d8dee3fc02b89398608a40
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525127"
---
# <a name="bookingquestionassignment-resource-type"></a>тип ресурса bookingQuestionAssignment

Пространство имен: microsoft.graph

Содержит набор пользовательских вопросов, связанных с определенной службой.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isRequired|Boolean|ID настраиваемого вопроса.|
|questionId|Строка|Указывает, обязательно ли отвечать на настраиваемый вопрос.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingQuestionAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingQuestionAssignment",
  "questionId": "String",
  "isRequired": "Boolean"
}
```

