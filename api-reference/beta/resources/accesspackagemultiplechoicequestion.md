---
title: тип ресурса accessPackageMultipleChoiceQuestion
description: Подкласс accessPackageQuestion, который имеет несколько вариантов в формате ответа на вопрос
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1efcfabbbc345f5820ddaf90bcec9ba9c7076837
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468323"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a>тип ресурса accessPackageMultipleChoiceQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ребенок **accessPackageQuestion** , который представляет несколько вариантов, из чего должен выбрать ответ запросчик. Это используется в свойстве  [вопросов accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) и в [accessPackageResourceAttribute](accesspackageresourceattribute.md) ресурса пакета доступа.

Наследует от [accessPackageQuestion](../resources/accesspackagequestion.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allowsMultipleSelection|Логический|Указывает, может ли запросчик выбрать несколько вариантов в качестве ответа.|
|выбор|[accessPackageAnswerChoice collection](../resources/accesspackageanswerchoice.md)|Список вариантов ответов.|
|id|Строка|ID вопроса. Наследуется [от accessPackageQuestion](../resources/accesspackagequestion.md).|
|isRequired|Boolean|Указывает, требуется ли запросчику предоставить ответ или нет. Наследуется [от accessPackageQuestion](../resources/accesspackagequestion.md).|
|sequence|Int32|Относительное положение этого вопроса при отобраии списка вопросов для запросителя. Наследуется [от accessPackageQuestion](../resources/accesspackagequestion.md).|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса, чтобы показать запросчик. Наследуется [от accessPackageQuestion](../resources/accesspackagequestion.md).|

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
