---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта **subscribedSku** представляет собой коллекцию объектов servicePlanInfo.
localization_priority: Normal
ms.openlocfilehash: e759082984cc66f7d3efec3cbb7cbee11561f253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512607"
---
# <a name="serviceplaninfo-resource-type"></a>Тип ресурса servicePlanInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|servicePlanId|Guid|Уникальный идентификатор плана обслуживания.|
|servicePlanName|String|Имя плана обслуживания.|
|provisioningStatus|String|Состояние подготовки плана обслуживания. Возможные значения:<br/>"Success" — служба полностью подготовлена.<br/>"Disabled" — служба отключена.<br/>"PendingInput" — служба еще не подготовлена, ожидается подтверждение.<br/>«PendingActivation» - служба подготовки, но требует явные активации администратором (например, план обслуживания Intune_O365).<br/>"PendingProvisioning" — Майкрософт добавила в продукт новую службу, но она пока не активирована в клиенте.|
|appliesTo|String|Объект, которому может быть назначен план обслуживания. Возможные значения:<br/>"User" — план обслуживания можно назначить отдельным пользователям.<br/>"Company" — план обслуживания можно назначить всему клиенту.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/serviceplaninfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
