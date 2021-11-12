---
title: тип ресурса organizationSettings
description: Содержит параметры, применимые к организации или объектам пользователя в ней.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2c351cfe0f55ef7a2bfb1cf6d62a379ee335a644
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780585"
---
# <a name="organizationsettings-resource-type"></a>тип ресурса organizationSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит параметры, применимые к [организации](organization.md) или которые должны применяться к [объектам пользователей](user.md) в организации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получить параметры организации](../api/organizationsettings-get.md) | [organisationSettings](organizationsettings.md) | Ознакомьтесь с объектом параметры организации. |
| [Создание profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Создайте новый **профильCardProperty,** разместив в **коллекции объектов profileCardProperty.** |
| [List profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | [коллекция profileCardProperty](profilecardproperty.md) | Получите **коллекцию объектов profileCardProperty.** |
| [List itemInsights](../api/organizationsettings-list-iteminsights.md) | [insightsSettings](insightssettings.md) | Получите свойства объекта [insightsSettings](insightssettings.md) для отображения или возвращения элементов в организации. |
| [Список peopleInsights](../api/organizationsettings-list-peopleinsights.md) | [insightsSettings](insightssettings.md) | Получите свойства объекта [insightsSettings](insightssettings.md) для отображения или возвращения людей в организации. |


## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|id |String| Id объекта параметров для организации. |
|profileCardProperties|[коллекция profileCardProperty](profilecardproperty.md)| Содержит коллекцию свойств, которые администратор определил как видимые на Microsoft 365 профилей. [Получить параметры организации](../api/organizationsettings-get.md) возвращает свойства, настроенные для профилей для организации.|
|itemInsights|[insightsSettings](insightssettings.md)| Содержит свойства, настроенные администратором для видимости данных microsoft Graph, между пользователем и другими элементами в Microsoft 365, например документами или сайтами. [List itemInsights](../api/organizationsettings-list-iteminsights.md) возвращает _параметры_ для отображения или возврата элементов в организации.|
|peopleInsights|[insightsSettings](insightssettings.md)| Содержит свойства, настроенные администратором для видимости списка людей, [](/graph/people-example#including-a-person-as-relevant-or-working-with) соответствующих и работающих с пользователем в Microsoft 365. [Список peopleInsights](../api/organizationsettings-list-peopleinsights.md) возвращает _параметры_ для отображения или возврата понимания людей в организации.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


