---
title: Тип ресурса accessPackageAnswer
description: Сложный тип ответов на accessPackageQuestion, хранимый в accessPackageAssignmentRequest.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3da6d1b0e2e519895af4dacca009b027807b0184
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135508"
---
# <a name="accesspackageanswer-resource-type"></a>Тип ресурса accessPackageAnswer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип предоставленного запросителем ответа [accessPackageQuestion.](../resources/accesspackagequestion.md) Фактическим ответом будет подтип этого сложного [типа, accessPackageAnswerString](../resources/accesspackageanswerstring.md) или [accessPackageAnswerChoice.](../resources/accesspackageanswerchoice.md) Эти ответы будут сохранены в [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|Ответ на вопрос. Обязательно и только для чтения.|
|displayValue|Строка|Отображаемая величина ответа. Обязательный.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswer",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```

