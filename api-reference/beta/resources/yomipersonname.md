---
title: Тип ресурса Йомиперсоннаме
description: Тип ресурса Йомиперсоннаме
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8117dd71947fea41508ccbe7d50d49a4f78b335d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939770"
---
# <a name="yomipersonname-resource-type"></a>Тип ресурса Йомиперсоннаме

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет пользователю способ хранения сведений о том, как произношение имени для несобственных динамиков языка, в котором представлен ресурс [PersonName](personname.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                             |
|:-------------|:------------|:--------------------------------------------------------|
|displayName   |Строка       | Составные руководства по произношению имени и фамилии.  |
|первыми         |Строка       | Произношение руководства для первого имени пользователя.     |
|Фамили          |Строка       | Произношение руководства для последнего имени пользователя.      |
|маиден        |Строка       | Произношение руководства для маиден имени пользователя.    |
|назван        |Строка       | Произношение руководства по среднему имени пользователя.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.yomiPersonName",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "yomiPersonName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
