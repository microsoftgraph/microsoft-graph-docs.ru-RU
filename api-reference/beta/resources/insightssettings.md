---
title: тип ресурса insightsSettings
description: Представляет параметры конфиденциальности для анализа.
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c78b1e3c4836af0d93dccd1e21edeba69e07381a
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322766"
---
# <a name="insightssettings-resource-type"></a>тип ресурса insightsSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет _параметры для_ вычисления и управления отображением или программным возвращением определенного типа информации в организации. Сведения могут быть сведениями о элементах, сведениями о часах собраний или сведениями о человеке. 

Сведения о [элементах](https://support.microsoft.com/en-us/office/suggested-meeting-hours-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) и сведения о часах собраний представляют отношения между пользователями и элементами, такими как документы, сайты и другие типы контента в Microsoft 365. Программным образом они представлены ресурсом [itemInsights.](iteminsights.md) Вы можете получить документы, которые [делятся](../api/insights-list-shared.md) с пользователем, [](../api/insights-list-trending.md) в тренде вокруг пользователя или [используются](../api/insights-list-used.md) пользователем. Вы можете использовать **insightsSettings** для настройки параметров конфиденциальности для вычисления, отображения или возврата элементов в [организации.](/graph/insights-customize-item-insights-privacy)

Сведения о работе с людьми представляют собой связи людей, которые имеют отношение друг к другу или работают друг с другом на основе их связей с общественностью. Программным образом отдельные люди представлены ресурсом [person.](person.md) Вы можете [использовать API людей, чтобы получить сведения о человеке.](/graph/people-example) Вы можете использовать **insightsSettings** для настройки параметров конфиденциальности для отображения или возвращения [людей.](/graph/insights-customize-people-insights-privacy)

Напротив, для анализа элементов и времени собраний вы также можете управлять  их вычислением и видимостью на уровне пользователя с помощью [ресурса userInsightsSettings.](userinsightssettings.md) [](https://support.microsoft.com/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List itemInsights](../api/organizationsettings-list-iteminsights.md) | [insightsSettings](insightssettings.md) | Получите _параметры в_ [объекте insightsSettings](insightssettings.md) для отображения элементов в организации. |
| [Список peopleInsights](../api/organizationsettings-list-peopleinsights.md) | [insightsSettings](insightssettings.md) | Получите _параметры в_ [объекте insightsSettings](insightssettings.md) для отображения понимания людей в организации. |
| [Обновление insightsSettings](../api/insightssettings-update.md) | [insightsSettings](insightssettings.md) | Обнови свойства ресурса **insightsSettings** для управления отображением или возвращением указанного типа анализов, которые могут быть сведениями о элементах или сведениями людей. |


## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` если для организации включен указанный тип анализа; если указанный тип анализа отключен для `false` всех пользователей без исключений. Значение по умолчанию: `true`. Необязательно.|
|disabledForGroup|Строка| ID группы Azure AD, в которой указанный тип данных отключен для ее участников. Значение по умолчанию: `empty`. Необязательно.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.insightsSettings"
}-->

```json
{

  "isEnabledInOrganization": "Boolean",
  "disabledForGroup": "String"
}
```





