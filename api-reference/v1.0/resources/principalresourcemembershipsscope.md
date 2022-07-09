---
title: Тип ресурса principalResourceMembershipsScope
description: Позволяет выбрать область проверки доступа для проверки доступа выбранных участников к выбранным ресурсам.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2f9c2982dd8b73969d9b51b2242ad2c33367031e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698074"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>Тип ресурса principalResourceMembershipsScope

Пространство имен: microsoft.graph

PrincipalResourceMembershipsScope — это тип [accessReviewScope](accessreviewscope.md) , который позволяет выбрать коллекцию основных областей и коллекцию областей ресурсов и проверить доступ выбранных субъектов к выбранным ресурсам. Он используется для настройки свойства **области** [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).

Наследуется [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|principalScopes|[Коллекция accessReviewScope](../resources/accessreviewscope.md)|Определяет области субъектов, доступ к ресурсам которых проверяются в проверке доступа.|
|resourceScopes|[Коллекция accessReviewScope](../resources/accessreviewscope.md)|Определяет области ресурсов, для которых проверяется доступ.|

Необходимо также указать **свойство @odata.type** со значением `#microsoft.graph.principalResourceMembershipsScope`. Дополнительные сведения о параметрах  конфигурации для области с помощью **principalResourceMembershipsScope** см. в статье "Настройка области определения проверки доступа с помощью microsoft [API Graph](/graph/accessreviews-scope-concept)".

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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
