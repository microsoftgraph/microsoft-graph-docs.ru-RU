---
title: licenseDetails тип ресурса
description: Содержит информацию о лицензии, назначенной пользователю.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 4e23dfcd15dc2b05a9d1c7356a532e6faf487662
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547192"
---
# <a name="licensedetails-resource-type"></a>licenseDetails тип ресурса

Пространство имен: microsoft.graph

Содержит информацию о лицензии, назначенной пользователю.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление licenseDetails](../api/user-list-licensedetails.md) | Коллекция объектов licenseDetails |Получить список объектов licenseDetails для пользователя.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор объекта детализации лицензии. Читать только, ключ, не сведены на нет |
|servicePlans|Коллекция [servicePlanInfo](serviceplaninfo.md)| Информация о планах обслуживания, назначенных лицензией. Читать только, не обнуляемый |
|skuId|Guid| Уникальный идентификатор (GUID) для службы SKU. Равно свойству skuId на связанном [объекте SubscribedSku.](subscribedsku.md) Только для чтения |
|skuPartNumber|String| Уникальное имя дисплея SKU. Равный skuPartNumber на связанном [объекте SubscribedSku;](subscribedsku.md) например: "AAD_Premium". Только для чтения |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

