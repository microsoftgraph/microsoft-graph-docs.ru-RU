---
title: Тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: 5236a73697ea6969698fa0cdb6a8368188d0271c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029199"
---
# <a name="licensedetails-resource-type"></a>Тип ресурса licenseDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о лицензии, назначенной пользователю.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление licenseDetails](../api/user-list-licensedetails.md) | Коллекция объектов licenseDetails |Получение списка объектов licenseDetails для пользователя.|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор для объекта сведений о лицензии. Только для чтения, ключ, не допускающий значение null |
|сервицепланс|Коллекция [servicePlanInfo](serviceplaninfo.md)| Сведения о планах обслуживания, назначенных с лицензией. Только для чтения, не допускает значение null |
|skuId|Guid| Уникальный идентификатор (GUID) для SKU службы. Равно свойству skuId в связанном объекте [SubscribedSku](subscribedsku.md) . Только для чтения |
|скупартнумбер|String| Имя уникального отображаемого номера SKU. Равно Скупартнумбер для связанного объекта [SubscribedSku](subscribedsku.md) ; Пример: "AAD_Premium". Только для чтения |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


