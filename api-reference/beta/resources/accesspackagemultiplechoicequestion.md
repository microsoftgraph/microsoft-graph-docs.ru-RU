---
title: Тип ресурса accessPackageMultipleChoiceQuestion
description: Подкласс accessPackageQuestion с множественным выбором в качестве формата ответа на вопрос
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab61a8df1faf0f9b1d9fa3dee10521001ddc6d31
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720377"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a>Тип ресурса accessPackageMultipleChoiceQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Child of **accessPackageQuestion,** который представляет несколько параметров, из которые запрашивает должен выбрать ответ.

Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowsMultipleSelection|Boolean|Указывает, может ли запросителем выбрать несколько вариантов в качестве ответа.|
|choices|[Коллекция accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md)|Список вариантов ответов.|
|id|String|ИД вопроса. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|
|isRequired|Boolean|Указывает, требуется ли запрашивать ответ. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|
|sequence|Int32|Относительное положение этого вопроса при отобралчику списка вопросов. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса для показа запросителем. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "choices": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
    }
  ],
  "allowsMultipleSelection": "Boolean"
}
```
