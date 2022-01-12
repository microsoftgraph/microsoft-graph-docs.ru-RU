---
title: тип ресурса accessPackageQuestion
description: Сложный тип для вопросов, настроенных в политике назначения пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: df4158f7869407772b0c7a8807366d03e2ef7a62
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791947"
---
# <a name="accesspackagequestion-resource-type"></a>тип ресурса accessPackageQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для свойства политики назначения `accessPackageQuestion` [пакета доступа.](accesspackageassignmentpolicy.md) 

Подтипы включают [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) и [accessPackageMultipleChoiceQuestions.](accesspackagemultiplechoicequestion.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String| ID вопроса.|
|isRequired|Boolean| Требуется ли запросчику предоставить ответ или нет.|
|sequence|Int32| Относительное положение этого вопроса при отобраии списка вопросов для запросителя.|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса, который нужно показать запросчику.|
|isAnswerEditable|Логический| Указывает, разрешено ли запросчику изменять ответы на вопросы.|

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