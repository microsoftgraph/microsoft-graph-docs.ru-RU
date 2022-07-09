---
title: Тип ресурса accessReviewQueryScope
description: Определяет, что необходимо проверить при проверке доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84c89344ffbb043ee839b2c228a691c2c47e7c32
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696506"
---
# <a name="accessreviewqueryscope-resource-type"></a>Тип ресурса accessReviewQueryScope

Пространство имен: microsoft.graph

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
