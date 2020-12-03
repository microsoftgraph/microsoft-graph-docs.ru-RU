---
title: Тип ресурса Итеминсигхтссеттингс
description: Представляет параметры конфиденциальности для Итеминсигхтс.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c84b2397c938997a3285d16612d090ae22444580
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522771"
---
# <a name="iteminsightssettings-resource-type"></a>Тип ресурса Итеминсигхтссеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры конфиденциальности для [итеминсигхтс](iteminsights.md) и параметров конфиденциальности для отслеживания времени проведения собрания. Используйте этот API, чтобы отключить или включить вычисление и видимость данных об объеме и времени собраний. 

- Application Insights: вычисляет отношения между пользователями и элементами, такими как документы или сайты в Microsoft 365.  
- Сведения о часах собраний: вычисляет время собрания в календаре пользователя на основе действий в Word, Excel, PowerPoint, электронной почте и календаре Outlook в Microsoft 365.

> [!NOTE]
> Сведения о времени проведения собраний выходят на клиентов, начиная с ноября 2020. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [получение](../api/iteminsightssettings-get.md);| [итеминсигхтссеттингс](iteminsightssettings.md) | Чтение свойств объекта **итеминсигхтссеттингс** . |
| [обновление](../api/iteminsightssettings-update.md).| [итеминсигхтссеттингс](iteminsightssettings.md) | Обновление объекта **итеминсигхтссеттингс** .|


## <a name="properties"></a>Свойства
| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Логический| `true` , если аналитика элемента организации включена; `false` Если аналитика элемента Организации отключена для всех пользователей без исключений. Значение по умолчанию: `true`. Необязательный параметр.|
|disabledForGroup|String| Идентификатор группы Azure AD, для которой отключается аналитика элемента "участники". Значение по умолчанию: `empty`. Необязательный параметр.|

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


