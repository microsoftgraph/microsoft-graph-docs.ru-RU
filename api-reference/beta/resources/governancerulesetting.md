---
title: Тип ресурса governanceRuleSetting
description: Представляет правила, которые предоставляют параметры роли.
localization_priority: Normal
ms.openlocfilehash: 7554c96daec70a95cde5ab0c3faedfba74764cff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894259"
---
# <a name="governancerulesetting-resource-type"></a>Тип ресурса governanceRuleSetting

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет правила, которые предоставляют параметры роли.


## <a name="properties"></a>Свойства
|Свойство      | Тип         |Описание|
|:-------------|:-------------|:----------|
|ruleIdentifier|Строка        |Идентификатор правила. Например ``ExpirationRule`` и ``MfaRule``.|
|setting       |String        |Параметры правила. Значение — это строка JSON со списком пар в формате Parameter_Name:Parameter_Value. Например, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
