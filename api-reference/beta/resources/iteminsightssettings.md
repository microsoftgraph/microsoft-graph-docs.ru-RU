---
title: тип ресурса itemInsightsSettings
description: Представляет параметры конфиденциальности для itemInsights.
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 764e47071d0f7554e3bcdd2c5ce4350304bdd6fe
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891232"
---
# <a name="iteminsightssettings-resource-type"></a>тип ресурса itemInsightsSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры конфиденциальности [для itemInsights и](iteminsights.md) параметр конфиденциальности для анализа [часов собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) Используйте этот API, чтобы отключить/включить вычисление и обзор информации о элементах и сведения о часах собраний. 

- Сведения о элементах. Вычисляется связь между пользователями и элементами, такими как документы или сайты в Microsoft 365.  
- Сведения о часах собраний: вычисляет часы собраний календаря на основе действий в Word, Excel, PowerPoint, электронной почте и Outlook в Microsoft 365.

Используйте [ресурс userInsightsSettings,](userinsightssettings.md) чтобы отключить и включить вычисления и видимость озарения элементов и сведения о часах собраний пользователя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [получение](../api/iteminsightssettings-get.md);| [itemInsightsSettings](iteminsightssettings.md) | Ознакомьтесь с свойствами **объекта itemInsightsSettings.** |
| [Обновление](../api/iteminsightssettings-update.md)| [itemInsightsSettings](iteminsightssettings.md) | Обновление **объекта itemInsightsSettings.**|


## <a name="properties"></a>Свойства
| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Логическое| `true` если включена информация о элементах организации; `false` если сведения о элементах организации отключены для всех пользователей без исключений. Значение по умолчанию: `true`. Необязательное.|
|disabledForGroup|String| ID группы Azure AD, из которой отключены сведения о элементах участников. Значение по умолчанию: `empty`. Необязательное.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.itemInsightsSettings"
}-->

```json
{
  "isEnabledInOrganization": "Boolean",
  "disabledForGroup": "String"
}
```


