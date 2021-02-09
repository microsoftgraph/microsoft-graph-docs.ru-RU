---
title: Тип ресурса organizationSettings
description: Содержит параметры, применимые к организации или объектам-пользователям в ней.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 105a57c7cb5827e9017df7494d32802ef7ac6fa5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158326"
---
# <a name="organizationsettings-resource-type"></a>Тип ресурса organizationSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит параметры, применимые [](organization.md) к организации или применяемые к объектам [пользователей](user.md) в организации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получить параметры организации](../api/organizationsettings-get.md) | [organizationSettings](organizationsettings.md) | Чтение объекта параметров организации. |
| [Создание profileCardProperty](../api/organizationsettings-post-profilecardproperties.md) | [profileCardProperty](profilecardproperty.md) | Создание нового **объекта profileCardProperty** путем публикации в коллекции объектов **profileCardProperty.** |
| [List profileCardProperties](../api/organizationsettings-list-profilecardproperties.md) | [Коллекция profileCardProperty](profilecardproperty.md) | Получите **коллекцию объектов profileCardProperty.** |
| [Get itemInsightsSettings](../api/iteminsightssettings-get.md) | [itemInsightsSettings](iteminsightssettings.md) | Получите свойства объекта **itemInsightsSettings.** |
| [Обновление itemInsightsSettings](../api/iteminsightssettings-update.md) | [itemInsightsSettings](iteminsightssettings.md) | Обновление свойств указанного ресурса **itemInsightsSettings.** |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|id |String| ИД объекта параметров для организации. |
|profileCardProperties|[Коллекция profileCardProperty](profilecardproperty.md)| Содержит коллекцию свойств, которые администратор определил как видимые на карточке профиля Microsoft 365. [При этом возвращаются](../api/organizationsettings-get.md) свойства, настроенные для карт профилей организации.|
|itemInsights|[itemInsightsSettings](iteminsightssettings.md)| Содержит свойства, настроенные администратором для видимости данных, полученных от Microsoft Graph, между пользователем и другими элементами в Microsoft 365, такими как документы или сайты. [Получите itemInsightsSettings через](../api/iteminsightssettings-get.md) это свойство навигации.|

## <a name="json-representation"></a>Представление JSON

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


