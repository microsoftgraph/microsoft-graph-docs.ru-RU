---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547461"
---
# <a name="governancerulesetting-resource-type"></a>Тип ресурса Говернанцерулесеттинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет правила, из которых состоят параметры ролей.


## <a name="properties"></a>Свойства
|Свойство      | Тип         |Описание|
|:-------------|:-------------|:----------|
|Рулеидентифиер|String        |Идентификатор правила. Например, ``ExpirationRule`` и ``MfaRule``.|
|setting       |String        |Параметры правила. Значением является строка JSON со списком пар в формате Параметер_наме: Параметер_валуе. Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerulesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
