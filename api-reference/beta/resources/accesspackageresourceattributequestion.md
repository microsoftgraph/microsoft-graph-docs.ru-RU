---
title: тип ресурса accessPackageResourceAttributeQuestion
description: Ресурс, определяющий вопрос, предоставляемый конечному пользователю, для получения значения атрибута, которое будет передано в итоге системе или в утвержденную заявку.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5ced0c1e769000f3624681d92dade18cf8dddcc9
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468294"
---
# <a name="accesspackageresourceattributequestion-resource-type"></a>тип ресурса accessPackageResourceAttributeQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс, определяющий вопрос[](accesspackagequestion.md), предоставляемый конечному пользователю, для получения значения атрибута, которое будет передано в итоге системе или в утвержденную заявку.

Этот тип наследуется из [accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md) и используется в свойстве **attributeSource** [accessPackageResourceAttribute](accesspackageresourceattribute.md).

Единственным свойством является **вопрос**, который может быть [accessPackageTextInputQuestion](accesspackagetextinputquestion.md) или [тип объекта accessPackageMultipleChoiceQuestion](accesspackagemultiplechoicequestion.md) .

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|вопрос|accessPackageQuestion|Вопрос, заданный для получения значения атрибута|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttributeQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttributeQuestion",
  "question": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```
