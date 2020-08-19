---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта subscribedSku представляет собой коллекцию объектов **servicePlanInfo**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: bf27255c2e5d52cfa1b0fb6529dc7d4fa949deda
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808643"
---
# <a name="serviceplaninfo-resource-type"></a>Тип ресурса servicePlanInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|сервицепланид|Guid|Уникальный идентификатор плана обслуживания.|
|сервицепланнаме|String|Имя плана обслуживания.|
|provisioningStatus|String|Состояние подготовки плана обслуживания. Возможные значения:<br/>"Success" — служба полностью подготовлена.<br/>"Disabled" — служба отключена.<br/>"PendingInput" — служба еще не подготовлена; ожидается подтверждение службы.<br/>"Пендингактиватион" — служба подготовлена, но требует явной активации администратором (например, Intune_O365 план обслуживания).<br/>"Пендингпровисионинг" — Корпорация Майкрософт добавила новую службу в SKU продукта и еще не активировалась в клиенте.|
|Тег|String|Объект, которому можно назначить план обслуживания. Возможные значения:<br/>"User" — план обслуживания можно назначить отдельным пользователям.<br/>"Company" — план обслуживания можно назначить всему клиенту.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
