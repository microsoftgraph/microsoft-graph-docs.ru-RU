---
title: Тип ресурса Йомиперсоннаме
description: Тип ресурса Йомиперсоннаме
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a598c4b5e999b03aeb7201c6eae3a230d3160a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518975"
---
# <a name="yomipersonname-resource-type"></a>Тип ресурса Йомиперсоннаме

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет пользователю способ хранения сведений о том, как произношение имени для несобственных динамиков языка, в котором представлен ресурс [PersonName](personname.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание                                             |
|:-------------|:------------|:--------------------------------------------------------|
|displayName   |String       | Составные руководства по произношению имени и фамилии.  |
|первыми         |String       | Произношение руководства для первого имени пользователя.     |
|Фамили          |String       | Произношение руководства для последнего имени пользователя.      |
|маиден        |String       | Произношение руководства для маиден имени пользователя.    |
|назван        |String       | Произношение руководства по среднему имени пользователя.    |

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
