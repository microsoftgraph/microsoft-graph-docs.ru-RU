---
title: тип ресурса accessReviewQueryScope
description: Определяет, что будет рассмотрено в обзоре доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 07a13d12b821d055c8200da2fa5450958a8f53ee
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579282"
---
# <a name="accessreviewqueryscope-resource-type"></a>тип ресурса accessReviewQueryScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Объект accessReviewQueryScope определяет, что будет рассмотрено в [обзоре доступа.](../resources/accessreviewsv2-root.md) Чтобы просмотреть обзор доступа для неактивных пользователей, см. [в примере accessReviewInactiveUserQueryScope.](../resources/accessreviewinactiveusersqueryscope.md) 

Наследует [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Запрос|Строка|Запрос, представляющий то, что будет рассмотрено в обзоре доступа.|
|queryRoot|Строка|В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса. Это свойство необходимо только в том случае, если указан относительный запрос. Например, `./manager`.|
|queryType|Строка|Указывает тип запроса. Типы включают `MicrosoftGraph` и `ARM` .|

Настоятельно рекомендуется **указать свойство @odata.type** со `#microsoft.graph.accessReviewQueryScope` значением. Дополнительные информацию о  параметрах конфигурации области с помощью **accessReviewQueryScope** см. в меню Настройка области определения обзора доступа с помощью [API Microsoft Graph.](/graph/accessreviews-scope-concept)

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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
