---
title: Тип ресурса accessReviewQueryScope
description: Определяет, что будет проверяться при проверке доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6fb31d3b040177e1065355bab7756b5bdf20ae02
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697872"
---
# <a name="accessreviewqueryscope-resource-type"></a>Тип ресурса accessReviewQueryScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Объект accessReviewQueryScope определяет, что будет проверяться при [проверке доступа](../resources/accessreviewsv2-overview.md). Сведения о том, как ограничить проверку доступа для неактивных пользователей, см. в [разделе accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md). 

Наследуется [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Запрос|Строка|Запрос, представляющий, что будет проверяться при проверке доступа.|
|queryRoot|Строка|В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для определения относительного источника запроса. Это свойство требуется только в том случае, если указан относительный запрос. Например, `./manager`.|
|queryType|Строка|Указывает тип запроса. Типы включают и `MicrosoftGraph` `ARM`.|

Настоятельно рекомендуется **указать свойство @odata.type** `#microsoft.graph.accessReviewQueryScope` со значением. Дополнительные сведения о параметрах  конфигурации области с помощью **accessReviewQueryScope** см. в статье "Настройка области определения проверки доступа с помощью microsoft [API Graph"](/graph/accessreviews-scope-concept).

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
