---
title: тип ресурса userInsightsSettings
description: Представляет параметры конфиденциальности пользователей для анализа элементов и данных о часах собраний.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5ecc9277d0bd98df99387a5dd222998074c6eb1b
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109217"
---
# <a name="userinsightssettings-resource-type"></a>тип ресурса userInsightsSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры конфиденциальности пользователей [для itemInsights](iteminsights.md) и [собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) Используйте этот ресурс, чтобы отключить/включить вычисления и видимость данных о элементах и сведения о часах собраний пользователя. 

- Сведения о элементах. Вычисляется связь между пользователями и элементами, такими как документы или сайты в Microsoft 365.  
- Сведения о часах собраний: вычисляет часы собраний календаря на основе действий в Word, Excel, PowerPoint, электронной почте и Outlook в Microsoft 365.

Используйте [ресурс itemInsightsSettings,](iteminsightssettings.md) чтобы отключить/включить вычисления и видимость анализа элементов и сведения о часах собраний на уровне организации.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                   | Описание                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [получение](../api/userinsightssettings-get.md);       | [userInsightsSettings](userinsightssettings.md) | Ознакомьтесь с свойствами **объекта userinsightsettings.**  |
| [Обновление](../api/userinsightssettings-update.md) | [userInsightsSettings](userinsightssettings.md) | Обновление свойств объекта **userinsightsettings.** |

## <a name="properties"></a>Свойства
| Свойство                   | Тип                                                  | Описание                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| isEnabled     | Boolean  |  `true` если включены **сведения о элементах itemInsights и** часах собраний; `false` если сведения о **элементах itemInsights и** время собраний отключены. Значение по умолчанию: `true`. Необязательно.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.userInsightsSettings"
}-->

```json
{
  "isEnabled": "Boolean"
}
```


