---
title: тип ресурса principalResourceMembershipsScope
description: Позволяет выбрать область обзора доступа, чтобы просмотреть доступ выбранных директоров к выбранным ресурсам.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d4e30ccccedb5dda72c4d0bb168655e1a8aedfd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019218"
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
