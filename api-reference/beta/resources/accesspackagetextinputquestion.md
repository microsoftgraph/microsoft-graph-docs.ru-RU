---
title: тип ресурса accessPackageTextInputQuestion
description: Ребенок accessPackageQuestion с текстовым вводом в формате ответа на вопрос.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0dee144139113716257ee1f41b6e585d22dc26b9
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468283"
---
# <a name="accesspackagetextinputquestion-resource-type"></a>тип ресурса accessPackageTextInputQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ребенок **accessPackageQuestion** с текстовым вводом в качестве ответа.  Это используется в свойстве  [вопросов accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) и в [accessPackageResourceAttribute](accesspackageresourceattribute.md) ресурса пакета доступа.

Наследует от [accessPackageQuestion](../resources/accesspackagequestion.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID вопроса. Наследуется [от accessPackageQuestion](../resources/accesspackagequestion.md).|
|isRequired|Boolean|Указывает, требуется ли запросчику предоставить ответ или нет. Наследуется [от accessPackageQuestion](../resources/accesspackagequestion.md).|
|isSingleLineQuestion|Логическое|Указывает, будет ли ответ в формате одной или нескольких строк.|
|sequence|Int32|Относительное положение этого вопроса при отобраии списка вопросов для запросителя. Наследуется [от accessPackageQuestion](../resources/accesspackagequestion.md).|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса, который нужно показать запросчику. Наследуется [от accessPackageQuestion](../resources/accesspackagequestion.md).|

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

