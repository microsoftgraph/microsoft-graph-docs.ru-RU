---
title: Тип ресурса accessPackageAnswerString
description: Ответ на строку accessPackageTextInputQuestion
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: def7753e62239e403821ed6472b3613d025942ac
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132407"
---
# <a name="accesspackageanswerstring-resource-type"></a>Тип ресурса accessPackageAnswerString

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает ответ на ввод строки [для accessPackageTextInputQuestion.](../resources/accesspackagetextinputquestion.md) Хранится в [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)

Наследуется от [accessPackageAnswer](../resources/accesspackageanswer.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|answeredQuestion|[accessPackageQuestion](../resources/accesspackagequestion.md)|Вопрос, к который применяется ответ. Наследуется от [accessPackageAnswer](../resources/accesspackageanswer.md).|
|displayValue|Строка|Локализованные отображаемые значения, которые отображаются для запрашивающих и утвержденных. Наследуется от [accessPackageAnswer](../resources/accesspackageanswer.md).|
|value|String|Значение, сохраненное в профиле пользователя запросителя, если этот ответ настроен для хранения в качестве определенного атрибута.|

## <a name="relationships"></a>Связи
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

