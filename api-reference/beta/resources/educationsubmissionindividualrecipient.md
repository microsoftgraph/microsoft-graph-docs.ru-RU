---
title: Тип ресурса educationSubmissionIndividualRecipient
description: 'Подкласс educationSubmissionRecipient, которое указывает, что отправка назначен одному пользователю в классе.  '
author: dipakboyed
ms.openlocfilehash: 3447c91fe4f387508a3afdf80a7337786d46f860
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318804"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a>Тип ресурса educationSubmissionIndividualRecipient

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Подкласс [educationSubmissionRecipient](educationsubmissionrecipient.md) , которое указывает, что отправка назначен одному пользователю в классе.  


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|userId|String|Идентификатор пользователя, которому назначена подачи.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->