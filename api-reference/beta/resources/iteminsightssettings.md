---
title: Тип ресурса Итеминсигхтссеттингс
description: Представляет параметры конфиденциальности для Итеминсигхтс.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3be5fa87fd6c2623126437fccb1ea43b7bc275f2
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427550"
---
# <a name="iteminsightssettings-resource-type"></a>Тип ресурса Итеминсигхтссеттингс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры конфиденциальности для [итеминсигхтс](iteminsights.md), которые настраивают видимость аналитических данных, полученных от Microsoft Graph, между пользователями и другими элементами (например, документами или сайтами) в Microsoft 365.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [получение](../api/iteminsightssettings-get.md);| [итеминсигхтссеттингс](iteminsightssettings.md) | Чтение свойств объекта **итеминсигхтссеттингс** . |
| [обновление](../api/iteminsightssettings-update.md).| [итеминсигхтссеттингс](iteminsightssettings.md) | Обновление объекта **итеминсигхтссеттингс** .|


## <a name="properties"></a>Свойства
| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|исенаблединорганизатион|Boolean| `true`, если аналитика элемента организации включена; `false`Если аналитика элемента Организации отключена для всех пользователей без исключений. Значение по умолчанию: `true`. Необязательное.|
|дисабледфорграуп|String| Идентификатор группы Azure AD, для которой отключается аналитика элемента "участники". Значение по умолчанию: `empty`. Необязательное.|

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
