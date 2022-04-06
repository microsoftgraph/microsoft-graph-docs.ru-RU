---
title: тип ресурсов governanceRuleSetting
description: Представляет правила, из которого состоят параметры ролей.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 212bee0fdf42e66346aef32083f86f748801ded1
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509674"
---
# <a name="governancerulesetting-resource-type"></a>тип ресурсов governanceRuleSetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Представляет правила, из которого состоят параметры ролей.


## <a name="properties"></a>Свойства
|Свойство      | Тип         |Описание|
|:-------------|:-------------|:----------|
|ruleIdentifier|String        |Id правила. Например, ``ExpirationRule`` и ``MfaRule``.|
|setting       |String        |Параметры правила. Это значение — строка JSON со списком пар в формате Parameter_Name:Parameter_Value. Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

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


