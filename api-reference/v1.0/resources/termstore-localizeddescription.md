---
title: локализованный тип ресурсаDescription
description: Представляет локализованное описание, используемое для описания термина в магазине терминов.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: ea44c35e4b8f7dd5eb1eadc7cbb6e4861a402b4d
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58515055"
---
# <a name="localizeddescription-resource-type"></a>локализованный тип ресурсаDescription

Пространство имен: microsoft.graph.termStore

Представляет локализованное описание, используемое для описания [термина] в магазине [терминов.]


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание на локализованных языках.|
|LanguageTag|Строка|Тег языка для метки.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.termStore.localizedDescription"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.localizedDescription",
  "description": "String",
  "languageTag": "String"
}
```

[microsoft.graph.termStore.term]: termStore-term.md
[microsoft.graph.termStore.store]: termStore-store.md
[термин]: ../resources/termstore-term.md
[магазин]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "TermLocalizedDescriptionFacet is the facet for containing the description of a set",
  "keywords": "termLocalizedDescriptionFacet,facet,resource",
  "section": "documentation",
  "tocPath": "TermLocalizedDescriptionFacet",
  "tocBookmarks": {
    "Resources/termStore.termLocalizedDescription&quot;: &quot;#"
  },
  "suppressions": []
}
-->


