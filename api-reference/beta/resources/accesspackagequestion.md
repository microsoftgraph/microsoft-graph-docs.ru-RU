---
title: Тип ресурса accessPackageQuestion
description: Сложный тип для вопросов, настроенных в политике назначения пакета доступа.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 04849b79cfa6c58132360f8ec20c363ea21453ec
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132399"
---
# <a name="accesspackagequestion-resource-type"></a>Тип ресурса accessPackageQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для `accessPackageQuestion` свойства политики назначения пакета [доступа.](accesspackageassignmentpolicy.md) 

Подтипы включают [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) и [accessPackageMultipleChoiceQuestions.](accesspackagemultiplechoicequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка| ИД вопроса.|
|isRequired|Boolean| Требуется ли запрашивать ответ.|
|sequence|Int32| Относительное положение этого вопроса при отобралчику списка вопросов.|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса, который необходимо показать запрашиваемой информации.|

## <a name="relationships"></a>Связи
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

