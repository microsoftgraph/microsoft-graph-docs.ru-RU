---
title: тип ресурса accessReviewQueryScope
description: Определяет, что необходимо просмотреть в обзоре доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cc6a8453b804e33eff2788b280928219ddf191cec4f49d2cb1b8c76725eab7c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180910"
---
# <a name="accessreviewqueryscope-resource-type"></a>тип ресурса accessReviewQueryScope

Пространство имен: microsoft.graph

Объект accessReviewQueryScope определяет то, что просматривается в [обзоре доступа.](../resources/accessreviewsv2-root.md) Чтобы просмотреть обзор доступа для неактивных пользователей, см. [в примере accessReviewInactiveUserQueryScope.](../resources/accessreviewinactiveusersqueryscope.md) 

Наследует [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Запрос|String|Запрос, представляющий то, что будет рассмотрено в обзоре доступа.|
|queryRoot|String|В сценарии, в котором рецензенты должны быть указаны динамически, это свойство используется для указать относительный источник запроса. Это свойство необходимо только в том случае, если указан относительный запрос. Например, `./manager`.|
|queryType|String|Указывает тип запроса. Типы включают `MicrosoftGraph` и `ARM` .|

Настоятельно рекомендуется **указать свойство @odata.type** со `#microsoft.graph.accessReviewQueryScope` значением. Дополнительные информацию о  параметрах конфигурации области с помощью **accessReviewQueryScope** см. в меню Настройка области определения обзора доступа с помощью [API Microsoft Graph.](/graph/accessreviews-scope-concept)

## <a name="relationships"></a>Связи
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
