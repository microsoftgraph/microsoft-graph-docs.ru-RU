---
title: Тип ресурса servicePlanInfo
description: Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта subscribedSku представляет собой коллекцию объектов **servicePlanInfo**.
ms.localizationpriority: medium
author: jpettere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a9b1f3d2aa6fbadd1b15686e5c5126635cba0873
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348945"
---
# <a name="serviceplaninfo-resource-type"></a>Тип ресурса servicePlanInfo

Пространство имен: microsoft.graph

Содержит сведения о плане обслуживания, связанном с подписанным SKU. Свойство **servicePlans** объекта [subscribedSku](subscribedsku.md) представляет собой коллекцию объектов **servicePlanInfo**.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|servicePlanId|Guid|Уникальный идентификатор плана обслуживания.|
|servicePlanName|String|Имя плана обслуживания.|
|provisioningStatus|String|Состояние подготовки плана обслуживания. Возможные значения:<br/>`Success` - Служба полностью готова.<br/>`Disabled` - Служба отключена.<br/>`ErrorStatus` - План службы не был предусмотрен и находится в состоянии ошибки.<br/>`PendingInput` - служба еще не предусмотрена; ожидание подтверждения службы.<br/>`PendingActivation` - Служба является предварительной, но требует явной активации администратором (например, Intune_O365 плана службы)<br/>`PendingProvisioning` - Корпорация Майкрософт добавила новую службу в SKU продукта, и она еще не была активирована в клиенте.|
|appliesTo|String|Объект, на который может быть назначен план службы. Возможные значения:<br/>`User` - план службы может быть назначен отдельным пользователям.<br/>`Company` - план службы может быть назначен для всего клиента.|

## <a name="json-representation"></a>Представление JSON

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
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

