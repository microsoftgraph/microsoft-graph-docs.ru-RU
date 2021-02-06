---
title: Тип ресурса accessPackageTextInputQuestion
description: Child of accessPackageQuestion that has text input as the question's answer format.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5f7d4d0ee7517ec3455d9e63647461e8101cab9d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133580"
---
# <a name="accesspackagetextinputquestion-resource-type"></a>Тип ресурса accessPackageTextInputQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Child of **accessPackageQuestion** that has text input as an answer.

Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ИД вопроса. Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)|
|isRequired|Boolean|Указывает, требуется ли запрашивать ответ. Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)|
|isSingleLineQuestion|Boolean|Указывает, будет ли ответ в формате одной или нескольких строк.|
|sequence|Int32|Относительное положение этого вопроса при отобралчику списка вопросов. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса, который должен показать запросителем. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageTextInputQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "isSingleLineQuestion": "Boolean"
}
```

