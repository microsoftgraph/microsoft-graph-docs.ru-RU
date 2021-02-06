---
title: Тип ресурса accessPackageMultipleChoiceQuestion
description: Подкласс accessPackageQuestion с множественным выбором в качестве формата ответа вопроса
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 54054edcda2f41ad3f4e1bd29fb807c18709ee1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137342"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a>Тип ресурса accessPackageMultipleChoiceQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Child of **accessPackageQuestion,** который представляет несколько параметров, из них запрашивает запрос.

Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowsMultipleSelection|Boolean|Указывает, может ли запросителем выбрать несколько вариантов в качестве ответа.|
|choices|[Коллекция accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md)|Список вариантов ответов.|
|id|Строка|ИД вопроса. Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)|
|isRequired|Boolean|Указывает, требуется ли запрашивать ответ. Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)|
|sequence|Int32|Относительное положение этого вопроса при отобралчику списка вопросов. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса для показа запросителем. Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)|

## <a name="relationships"></a>Связи
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
