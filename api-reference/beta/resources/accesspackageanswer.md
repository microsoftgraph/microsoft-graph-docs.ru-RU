---
title: Тип ресурса accessPackageAnswer
description: Сложный тип ответов на accessPackageQuestion, хранимый в accessPackageAssignmentRequest.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f947c5235c18d3be5115199d789512602a3e0739
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720383"
---
# <a name="accesspackageanswer-resource-type"></a>Тип ресурса accessPackageAnswer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип предоставленного запросителем ответа [на accessPackageQuestion.](../resources/accesspackagequestion.md) Фактическим ответом будет подтип этого сложного [типа, accessPackageAnswerString](../resources/accesspackageanswerstring.md) или [accessPackageAnswerChoice.](../resources/accesspackageanswerchoice.md) Эти ответы будут сохранены в [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|Вопрос, для ответа на который вы отвечаете. Обязательно и только для чтения.|
|displayValue|String|Отображаемая величина ответа. Обязательный.|

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

