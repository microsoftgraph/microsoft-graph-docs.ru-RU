---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 32be4465ffcd710bbfdaf8f3c60b3813a0b7d3be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497323"
---
# <a name="governancerulesetting-resource-type"></a>Тип ресурса Говернанцерулесеттинг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет правила, из которых состоят параметры ролей.


## <a name="properties"></a>Свойства
|Свойство      | Тип         |Описание|
|:-------------|:-------------|:----------|
|рулеидентифиер|String        |Идентификатор правила. Например, ``ExpirationRule`` и ``MfaRule``.|
|setting       |String        |Параметры правила. Значением является строка JSON со списком пар в формате Parameter_Name: Parameter_Value. Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

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
