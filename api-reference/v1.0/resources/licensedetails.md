---
title: Тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
ms.localizationpriority: medium
author: jconley76
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: bd5e7dfd7f6edcbf3cc7d79dcbfc4db9b0da7cfa
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549367"
---
# <a name="licensedetails-resource-type"></a>Тип ресурса licenseDetails

Пространство имен: microsoft.graph

Содержит сведения о лицензии, назначенной пользователю.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление licenseDetails](../api/user-list-licensedetails.md) | Коллекция объектов licenseDetails |Получение списка объектов licenseDetails для пользователя.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор объекта подробностей лицензии. Только для чтения, ключ, не допускает значения NULL |
|servicePlans|Коллекция [servicePlanInfo](serviceplaninfo.md)| Сведения о планах обслуживания, назначенных лицензией. Только для чтения, не допускает значение NULL |
|skuId|Guid| Уникальный идентификатор (GUID) для номера SKU службы. Равно свойству skuId связанного объекта [SubscribedSku](subscribedsku.md) . Только для чтения |
|skuPartNumber|String| Уникальное отображаемое имя SKU. Равно skuPartNumber для связанного объекта [SubscribedSku](subscribedsku.md) ; Например, "AAD_Premium". Только для чтения |

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

