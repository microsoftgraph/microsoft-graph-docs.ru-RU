---
title: тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: a8edde4e0e1e5df6e2fad7bcacca1fb67641d9b7
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853972"
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
|skuId|GUID| Уникальный идентификатор (GUID) для службы SKU. Равно свойству skuId на связанном [объекте SubscribedSku](subscribedsku.md) . Только для чтения |
|skuPartNumber|String| Уникальное имя отображения SKU. Равно skuPartNumber на связанном [объекте SubscribedSku](subscribedsku.md) ; например: "AAD_Premium". Только для чтения |

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
  "skuId": "GUID",
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

