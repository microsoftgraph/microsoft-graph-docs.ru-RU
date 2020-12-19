---
title: Тип ресурса accessPackageAnswerString
description: Ответ на строку accessPackageTextInputQuestion
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a5273872b2ded749ddfc13998c5b0104a0a63ec
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720293"
---
# <a name="accesspackageanswerstring-resource-type"></a>Тип ресурса accessPackageAnswerString

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает ответ на ввод строки [для accessPackageTextInputQuestion.](../resources/accesspackagetextinputquestion.md) Хранится в [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

Наследуется от [accessPackageAnswer.](../resources/accesspackageanswer.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|Вопрос, к который применяется ответ. Наследуется от [accessPackageAnswer](../resources/accesspackageanswer.md).|
|displayValue|String|Локализованные отображаемые значения, которые отображаются для запрашивающих и утвержденных. Наследуется от [accessPackageAnswer](../resources/accesspackageanswer.md).|
|value|String|Значение, сохраненное в профиле пользователя запросителя, если этот ответ настроен для хранения в качестве определенного атрибута.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerString",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  },
  "value": "String"
}
```

