---
title: тип ресурса recommendedAction
description: Представляет рекомендуемые действия для клиента на основе имитации атаки и учебной кампании по улучшению его осанки безопасности.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8932b20e38da6f544f9f9e668b8b304f49fbde6c
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979711"
---
# <a name="recommendedaction-resource-type"></a>тип ресурса recommendedAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет рекомендуемые действия для клиента на основе имитации атаки и учебной кампании по улучшению его осанки безопасности.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionWebUrl|Строка|Веб-URL-адрес рекомендуемого действия.|
|potentialScoreImpact|Двойное|Возможное улучшение показателей безопасности клиента в рекомендуемом действии.|
|title|String|Название рекомендуемого действия.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recommendedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recommendedAction",
  "actionWebUrl": "String",
  "title": "String",
  "potentialScoreImpact": "Double"
}
```

