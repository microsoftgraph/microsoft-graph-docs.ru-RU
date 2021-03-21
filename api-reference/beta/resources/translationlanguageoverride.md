---
title: тип ресурса translationLanguageOverride
description: Ресурс, представляющий запись в переопределяемом списке языка перевода.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c9fa8d600ee3fb503446965d78491563c4ceae2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954953"
---
# <a name="translationlanguageoverride-resource-type"></a>тип ресурса translationLanguageOverride

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет любые переопределения перевода для языка.

## <a name="properties"></a>Свойства

|Свойство             |Тип                                         |Описание                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|LanguageTag          |Строка                                       |Язык для применения переопределения.<br><br>Возвращается по умолчанию. Значение null не допускается.       |                   
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


