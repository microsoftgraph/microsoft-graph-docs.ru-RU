---
title: Тип ресурса itemInsights
description: Связи между пользователем и элементами, такими как документы в OneDrive для бизнеса, вычисляемые с использованием передовых методов анализа и машинного обучения. К примеру, вы можете определить документы OneDrive для бизнеса, пользующиеся популярностью у пользователей.
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 602cb58130f801e129bc334163cd7dabcc0d0b1b
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696983"
---
# <a name="iteminsights-resource-type"></a>Тип ресурса itemInsights

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Связи между пользователем и элементами, такими как документы в OneDrive для бизнеса, вычисляемые с использованием передовых методов анализа и машинного обучения. К примеру, вы можете определить документы OneDrive для бизнеса, пользующиеся популярностью у пользователей. Производный от [officeGraphInsights](officegraphinsights.md).

Аналитика возвращается с помощью указанных ниже API.

- [Популярные](insights-trending.md) — возвращает документы из OneDrive для бизнеса и сайтов SharePoint, популярные у пользователя.
- [Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем. Включает документы, использованные пользователем в OneDrive для бизнеса и SharePoint.
- [Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен общий доступ. Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.

Каждый объект аналитики возвращается со значением сложного типа (CVT) `resourceVisualization` и `resourceReference`. Значение CVT resourceVisualization содержит свойства, например `title` и `previewImageUrl`. Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.

### <a name="limiting-item-insights"></a>Ограничения для аналитики элементов

Обновите [itemInsightsSettings](iteminsightssettings.md), чтобы отключить аналитику элементов для определенной группы Azure AD или всей организации. Дополнительные сведения см. в статье [Настройка конфиденциальности для аналитики](/graph/insights-customize-item-insights-privacy?view=graph-rest-1.0).

## <a name="relationships"></a>Связи

| Связь      | Тип          | Описание  |
| ------------- |---------------| -------------|
| trending      | Коллекция объектов [trending](insights-trending.md)       | Вычисляемая связь, определяющая документы, популярные у пользователя. Документы, популярные у пользователя, рассчитываются на основе действий пользователя в ближайшей сети людей и включают файлы, сохраненные в OneDrive для бизнеса и SharePoint. Аналитика документов, популярных у пользователя, позволяет обнаружить потенциально полезное содержимое, к которому у пользователя есть доступ, но которое он еще не просматривал.|
| used      | Коллекция объектов [usedInsight](insights-used.md)        | Вычисляемая связь, определяющая последние документы, просмотренные и измененные пользователем, в том числе документы в OneDrive для бизнеса и SharePoint, упорядоченные по давности использования.|
| общие        | Коллекция объектов [sharedInsight](insights-shared.md)        | Вычисляемая связь, определяющая документы, к которым предоставлен общий доступ пользователю или пользователем, включает вложенные файлы в сообщениях электронной почты и собраниях, а также URL-адреса и ссылочные вложения в файлах OneDrive для бизнеса и SharePoint, которые можно найти в сообщениях электронной почты, собраниях и беседах Teams. Упорядочено по давности общего доступа.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.officeGraphInsights",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.itemInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```


