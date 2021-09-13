---
title: тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: ae262d8111c036fc4058cf8ace0b1f94fed4f132
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104112"
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

## <a name="relationships"></a>Отношения
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

