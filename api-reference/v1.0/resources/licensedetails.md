---
title: тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
localization_priority: Normal
author: jpettere
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 64bc8532e399be729c85200ca66b2f6e99b95084
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722232"
---
# <a name="licensedetails-resource-type"></a>тип ресурса licenseDetails

Пространство имен: microsoft.graph

Содержит сведения о лицензии, назначенной пользователю.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление licenseDetails](../api/user-list-licensedetails.md) | Коллекция объектов licenseDetails |Извлечение списка объектов licenseDetails для пользователя.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор объекта детализации лицензии. Только для чтения, клавиши, а не nullable |
|servicePlans|Коллекция [servicePlanInfo](serviceplaninfo.md)| Сведения о планах служб, присвоенных лицензией. Только для чтения, не является недействительным |
|skuId|Guid| Уникальный идентификатор (GUID) для службы SKU. Равно свойству skuId на связанном [объекте SubscribedSku.](subscribedsku.md) Только для чтения |
|skuPartNumber|String| Уникальное имя отображения SKU. Равно skuPartNumber на связанном [объекте SubscribedSku;](subscribedsku.md) например: "AAD_Premium". Только для чтения |

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

