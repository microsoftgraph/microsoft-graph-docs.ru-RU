---
title: Тип ресурса Итеминсигхтссеттингс
description: Представляет параметры конфиденциальности для Итеминсигхтс.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5d05a9fdf3a901fcddd55207bec373a3a0736afa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089331"
---
# <a name="iteminsightssettings-resource-type"></a>Тип ресурса Итеминсигхтссеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры конфиденциальности для [итеминсигхтс](iteminsights.md), которые настраивают видимость аналитических данных, полученных от Microsoft Graph, между пользователями и другими элементами (например, документами или сайтами) в Microsoft 365.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Получение](../api/iteminsightssettings-get.md)| [итеминсигхтссеттингс](iteminsightssettings.md) | Чтение свойств объекта **итеминсигхтссеттингс** . |
| [Обновление](../api/iteminsightssettings-update.md)| [итеминсигхтссеттингс](iteminsightssettings.md) | Обновление объекта **итеминсигхтссеттингс** .|


## <a name="properties"></a>Свойства
| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|isEnabledInOrganization|Boolean| `true` , если аналитика элемента организации включена; `false` Если аналитика элемента Организации отключена для всех пользователей без исключений. Значение по умолчанию: `true`. Необязательное свойство.|
|disabledForGroup|Строка| Идентификатор группы Azure AD, для которой отключается аналитика элемента "участники". Значение по умолчанию: `empty`. Необязательное свойство.|

## <a name="json-representation"></a>Представление в формате JSON

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


