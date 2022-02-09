---
title: тип ресурса accessPackageQuestion
description: Сложный тип для вопросов, настроенных в политике назначения пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 22e2cb56461830156d76c10f9e136a62dca4d440
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468309"
---
# <a name="accesspackagequestion-resource-type"></a>тип ресурса accessPackageQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется для **свойства accessPackageQuestion** политики назначения пакетов доступа и **accessPackageResourceAttributeQuestion** в [accessPackageResourceAttribute](accesspackageresourceattribute.md).[](accesspackageassignmentpolicy.md)

Подтипы включают [accessPackageTextInputQuestion](accesspackagetextinputquestion.md) и [accessPackageMultipleChoiceQuestion](accesspackagemultiplechoicequestion.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String| ID вопроса.|
|isRequired|Boolean| Требуется ли запросчику предоставить ответ или нет.|
|sequence|Int32| Относительное положение этого вопроса при отобраии списка вопросов для запросителя.|
|текст|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|Текст вопроса, который нужно показать запросчику.|
|isAnswerEditable|Логическое| Указывает, разрешено ли запросчику изменять ответы на вопросы.|

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