---
title: Тип ресурса ЕдукатионсубмиссиониндивидуалреЦипиент
description: 'Подкласс ЕдукатионсубмиссионреЦипиент, который указывает, что отправка назначена отдельному пользователю в классе.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8660ec569362d8170d15de86073c0ef59c9ec0a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507063"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a>Тип ресурса ЕдукатионсубмиссиониндивидуалреЦипиент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подкласс [едукатионсубмиссионреЦипиент](educationsubmissionrecipient.md) , который указывает, что отправка назначена отдельному пользователю в классе.  


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|userId|String|Идентификатор пользователя, которому назначена отправка.|

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
