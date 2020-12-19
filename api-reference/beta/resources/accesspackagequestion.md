---
title: Тип ресурса accessPackageQuestion
description: Сложный тип для вопросов, настроенных в политике назначения пакета доступа.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 876c21018104ed579cbaf04b0f4642395627964e
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720376"
---
# <a name="accesspackagequestion-resource-type"></a>Тип ресурса accessPackageQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для `accessPackageQuestion` свойства политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) 

Подтипы включают [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) и [accessPackageMultipleChoiceQuestions.](accesspackagemultiplechoicequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String| ИД вопроса.|
|isRequired|Boolean| Требуется ли запрашивать ответ.|
|sequence|Int32| Относительное положение этого вопроса при отобралчику списка вопросов.|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса, который необходимо показать запрашиваемой информации.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer"
}
```

