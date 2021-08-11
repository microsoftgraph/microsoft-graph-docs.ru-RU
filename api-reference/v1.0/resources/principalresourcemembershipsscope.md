---
title: тип ресурса principalResourceMembershipsScope
description: Позволяет выбрать область обзора доступа, чтобы просмотреть доступ выбранных директоров к выбранным ресурсам.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 494e4c24f0fa912190e60b74fdc1c39e09bb3dc32f8590b30e7391e770eb0d0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196560"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>тип ресурса principalResourceMembershipsScope

Пространство имен: microsoft.graph

PrincipalResourceMembershipsScope — это тип [accessReviewScope,](accessreviewscope.md) который позволяет выбрать коллекцию основных областей и коллекцию областей ресурсов и просмотреть доступ выбранных директоров к выбранным ресурсам. Он используется для настройки свойства **области** [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

Наследует [от accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|principalScopes|[коллекция accessReviewScope](../resources/accessreviewscope.md)|Определяет области директоров, доступ к ресурсам которых просматривается в обзоре доступа.|
|resourceScopes|[коллекция accessReviewScope](../resources/accessreviewscope.md)|Определяет области ресурсов, для которых просматривается доступ.|

Также необходимо указать **свойство @odata.type** со значением `#microsoft.graph.principalResourceMembershipsScope` . Дополнительные информацию о  параметрах конфигурации области с помощью **principalResourceMembershipsScope** см. в меню Настройка области определения обзора доступа с помощью [API](/graph/accessreviews-scope-concept)Microsoft Graph.

## <a name="relationships"></a>Связи
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
