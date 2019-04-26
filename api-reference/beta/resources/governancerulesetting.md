---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
ms.openlocfilehash: 433fc0d3ab3a524b86bbf1fc46dbe5185549473b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333732"
---
# <a name="governancerulesetting-resource-type"></a>Тип ресурса Говернанцерулесеттинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет правила, из которых состоят параметры ролей.


## <a name="properties"></a>Свойства
|Свойство      | Тип         |Описание|
|:-------------|:-------------|:----------|
|Рулеидентифиер|String        |Идентификатор правила. Например, ``ExpirationRule`` и ``MfaRule``.|
|setting       |String        |Параметры правила. Значением является строка JSON со списком пар в формате Параметер_наме: Параметер_валуе. Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

## <a name="json-representation"></a>Представление JSON

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
  "suppressions": []
}
-->
