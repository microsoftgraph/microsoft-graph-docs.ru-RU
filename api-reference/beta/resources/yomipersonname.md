---
title: Тип ресурса Йомиперсоннаме
description: Тип ресурса Йомиперсоннаме
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6e112d97f67b260c19de9fe0ab104e9dc1ed1d74
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810337"
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

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yomiPersonName"
}
-->

``` json

{
  "displayName": "String",
  "first": "String",
  "maiden": "String",
  "middle": "String",
  "last": "String"
}
```
