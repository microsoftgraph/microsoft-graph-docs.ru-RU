---
title: тип ресурса itemInsightsSettings
description: Представляет параметры конфиденциальности для itemInsights.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 80ca42440bcf365e051d9fb25fbc088af8a7f4bb
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108826"
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
|isEnabledInOrganization|Boolean| `true` если включена информация о элементах организации; `false` если сведения о элементах организации отключены для всех пользователей без исключений. Значение по умолчанию: `true`. Необязательно.|
|disabledForGroup|Строка| ID группы Azure AD, из которой отключены сведения о элементах участников. Значение по умолчанию: `empty`. Необязательно.|

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


