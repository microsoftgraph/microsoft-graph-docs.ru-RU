---
title: тип ресурса userInsightsSettings
description: Представляет параметры конфиденциальности пользователей для анализа элементов и данных о часах собраний.
ms.localizationpriority: medium
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: cd9e89e02b5ed36d0f5d3c16b7b667fa30bf75e2
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291073"
---
# <a name="userinsightssettings-resource-type"></a>тип ресурса userInsightsSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры конфиденциальности пользователей [для itemInsights](iteminsights.md) и [собраний](https://support.microsoft.com/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) . Используйте этот ресурс, чтобы отключить/включить вычисления и видимость данных о элементах и сведения о часах собраний пользователя. 

- Сведения о элементах. Вычисляется связь между пользователями и элементами, такими как документы или сайты в Microsoft 365.  
- Сведения о часах собраний: вычисляет часы собраний календаря на основе действий в Word, Excel, PowerPoint, электронной почте и Outlook в Microsoft 365.

Используйте [ресурс insightsSettings](insightssettings.md) , чтобы отключить/включить вычисления и видимость элементов, сведения о часах собраний или сведения о человеке на уровне организации.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                   | Описание                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [получение](../api/userinsightssettings-get.md);       | [userInsightsSettings](userinsightssettings.md) | Ознакомьтесь с свойствами **объекта userinsightsettings** .  |
| [Обновление](../api/userinsightssettings-update.md) | [userInsightsSettings](userinsightssettings.md) | Обновление свойств объекта **userinsightsettings** . |

## <a name="properties"></a>Свойства
| Свойство                   | Тип                                                  | Описание                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| isEnabled     | Boolean  |  `true` если включены **сведения о элементах itemInsights и** часах собраний; `false` если сведения о **элементах itemInsights и** время собраний отключены. Значение по умолчанию: `true`. Необязательный параметр.|

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


