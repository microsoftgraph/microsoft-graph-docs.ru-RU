---
title: тип ресурса principalResourceMembershipsScope
description: Позволяет для областей выбора просмотреть доступ выбранных директоров к выбранным ресурсам.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b22c52c0bf71f1a1169d51e2e6fd3e8ac10e99d9
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579895"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>тип ресурса principalResourceMembershipsScope

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

PrincipalResourceMembershipsScope — это тип [accessReviewScope,](accessreviewscope.md) который позволяет выбрать коллекцию основных областей и коллекцию областей ресурсов и просмотреть доступ выбранных директоров к выбранным ресурсам. Он используется для настройки свойства **области** [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

Наследует [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|principalScopes|[коллекция accessReviewScope](../resources/accessreviewscope.md)|Определяет области, включаемые в обзор доступа.|
|resourceScopes|[коллекция accessReviewScope](../resources/accessreviewscope.md)|Определяет области ресурсов, для которых будет рассмотрен доступ.|

Также необходимо указать **свойство @odata.type** со значением `#microsoft.graph.principalResourceMembershipsScope` . Дополнительные информацию о  параметрах конфигурации области с помощью **principalResourceMembershipsScope** см. в меню Настройка области определения обзора доступа с помощью [API](/graph/accessreviews-scope-concept)Microsoft Graph.

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
