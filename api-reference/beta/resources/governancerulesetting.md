---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 45ae44dccba67ee0b03f1941dd27795a002e810b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809532"
---
# <a name="governancerulesetting-resource-type"></a>Тип ресурса Говернанцерулесеттинг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет правила, из которых состоят параметры ролей.


## <a name="properties"></a>Свойства
|Свойство      | Тип         |Описание|
|:-------------|:-------------|:----------|
|рулеидентифиер|String        |Идентификатор правила. Например, ``ExpirationRule`` и ``MfaRule`` .|
|setting       |String        |Параметры правила. Значением является строка JSON со списком пар в формате Parameter_Name: Parameter_Value. Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`|

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
  "suppressions": []
}
-->
