---
title: тип ресурса userInsightsSettings
description: Представляет параметры конфиденциальности пользователей для анализа элементов и данных о часах собраний.
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 723f1ca8d0a56116039ae3f85eb0d534c3525972
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780893"
---
# <a name="userinsightssettings-resource-type"></a>тип ресурса userInsightsSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры конфиденциальности пользователей [для itemInsights](iteminsights.md) и [собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) Используйте этот ресурс, чтобы отключить/включить вычисления и видимость данных о элементах и сведения о часах собраний пользователя. 

- Сведения о элементах. Вычисляется связь между пользователями и элементами, такими как документы или сайты в Microsoft 365.  
- Сведения о часах собраний: вычисляет часы собраний календаря на основе действий в Word, Excel, PowerPoint, электронной почте и Outlook в Microsoft 365.

Используйте [ресурс insightsSettings,](insightssettings.md) чтобы отключить/включить вычисления и видимость элементов, сведения о часах собраний или сведения о человеке на уровне организации.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                   | Описание                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [получение](../api/userinsightssettings-get.md);       | [userInsightsSettings](userinsightssettings.md) | Ознакомьтесь с свойствами **объекта userinsightsettings.**  |
| [Update](../api/userinsightssettings-update.md) | [userInsightsSettings](userinsightssettings.md) | Обновление свойств объекта **userinsightsettings.** |

## <a name="properties"></a>Свойства
| Свойство                   | Тип                                                  | Описание                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| isEnabled     | Boolean  |  `true` если включены **сведения о элементах itemInsights и** часах собраний; `false` если сведения о **элементах itemInsights и** время собраний отключены. Значение по умолчанию: `true`. Необязательное.|

## <a name="json-representation"></a>Представление в формате JSON

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


