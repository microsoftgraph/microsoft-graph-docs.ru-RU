---
title: Тип ресурса accessPackageTextInputQuestion
description: Child of accessPackageQuestion that has text input as the question's answer format.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8609532e096fb587b4dcf49b8eb624aea314a8c6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720323"
---
# <a name="accesspackagetextinputquestion-resource-type"></a>Тип ресурса accessPackageTextInputQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Child of **accessPackageQuestion** that has text input as an answer.

Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД вопроса. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|
|isRequired|Boolean|Указывает, требуется ли запрашивать ответ. Наследуется [от accessPackageQuestion.](../resources/accesspackagequestion.md)|
|isSingleLineQuestion|Boolean|Указывает, будет ли ответ в формате одной или нескольких строк.|
|sequence|Int32|Относительное положение этого вопроса при отобралчику списка вопросов. Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса, который необходимо показать запрашиваемой информации. Наследуется от [accessPackageQuestion.](../resources/accesspackagequestion.md)|

## <a name="relationships"></a>Отношения
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

