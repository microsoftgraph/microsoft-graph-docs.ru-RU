---
title: тип ресурса insightsSettings
description: Представляет параметры конфиденциальности для анализа.
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 61625b4d9309ca203d1d523f1fcdb4f0fe6c583f
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500891"
---
# <a name="insightssettings-resource-type"></a>тип ресурса insightsSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет _параметры для_ вычисления и управления отображением или программным возвращением определенного типа информации в организации. Сведения могут быть сведениями о элементах, сведениями о часах собраний или сведениями о человеке. 

Сведения о элементах [](https://support.microsoft.com/office/suggested-meeting-hours-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) и сведения о часах собраний представляют отношения между пользователями и элементами, такими как документы, сайты и другие типы контента в Microsoft 365. Программным образом они представлены ресурсом [itemInsights](iteminsights.md) . Вы можете получить документы, [которые делятся](../api/insights-list-shared.md) с пользователем [, в](../api/insights-list-trending.md) тренде вокруг пользователя или [используются](../api/insights-list-used.md) пользователем. Вы можете использовать **insightsSettings** для настройки параметров конфиденциальности для вычисления, отображения или возврата элементов в [организации](/graph/insights-customize-item-insights-privacy).

Сведения о работе с людьми представляют собой связи людей, которые имеют отношение друг к другу или работают друг с другом на основе их связей с общественностью. Программным образом отдельные люди представлены ресурсом [person](person.md) . API [людей можно использовать для получения информации о человеке](/graph/people-example). Вы можете использовать **insightsSettings** для настройки параметров конфиденциальности для отображения или возвращения [людей.](/graph/insights-customize-people-insights-privacy)

Напротив, для анализа элементов и времени [](https://support.microsoft.com/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)собраний можно также управлять их расчетом и видимостью на уровне пользователя с помощью  [ресурса userInsightsSettings](userinsightssettings.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List itemInsights](../api/organizationsettings-list-iteminsights.md) | [insightsSettings](insightssettings.md) | Получите _параметры в_ [объекте insightsSettings](insightssettings.md) для отображения элементов в организации. |
| [Список peopleInsights](../api/organizationsettings-list-peopleinsights.md) | [insightsSettings](insightssettings.md) | Получите _параметры в_ [объекте insightsSettings](insightssettings.md) для отображения понимания людей в организации. |
| [Обновление insightsSettings](../api/insightssettings-update.md) | [insightsSettings](insightssettings.md) | Обнови свойства ресурса **insightsSettings** для управления отображением или возвращением указанного типа анализов, которые могут быть сведениями о элементах или сведениями людей. |


## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` если для организации включен указанный тип анализа; `false` если указанный тип анализа отключен для всех пользователей без исключений. Значение по умолчанию: `true`. Необязательный параметр.|
|disabledForGroup|String| ID группы Azure Active Directory, из которой указанный тип анализа отключен для ее участников. Значение по умолчанию: `empty`. Необязательный параметр.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.insightsSettings"
}-->

```json
{
  "disabledForGroup": "String",
  "isEnabledInOrganization": "Boolean"
}
```





