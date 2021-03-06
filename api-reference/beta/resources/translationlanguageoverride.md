---
title: тип ресурса translationLanguageOverride
description: Ресурс, представляющий запись в переопределяемом списке языка перевода.
localization_priority: Normal
author: jasonbro
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 791908546c64cbb0ea7ee7434bece3dca5c894cc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518172"
---
# <a name="translationlanguageoverride-resource-type"></a>тип ресурса translationLanguageOverride

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет любые переопределения перевода для языка.

## <a name="properties"></a>Свойства

|Свойство             |Тип                                         |Описание                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|LanguageTag          |String                                       |Язык для применения переопределения.<br><br>Возвращается по умолчанию. Значение null не допускается.       |                   
|translationBehavior  |[translationBehavior](translationPreferences.md#translationbehavior-values)        |Переопределять поведение перевода для языка, если таково.<br><br>Возвращается по умолчанию. Значение null не допускается.|

## <a name="json-representation"></a>Представление JSON

Ниже приводится определение ресурса JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationLanguageOverride"
}-->

```json
{
    "languageTag": "string",
    "translationBehavior": "string"
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationLanguageOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


