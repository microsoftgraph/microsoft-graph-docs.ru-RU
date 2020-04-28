---
title: Тип ресурса Привилежедролесеттингс
description: Представляет параметры привилегированной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c072f75095267910d128396c3848b2decca4728c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521497"
---
# <a name="privilegedrolesettings-resource-type"></a>Тип ресурса Привилежедролесеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры привилегированной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Чтение свойств и связей объекта Привилежедролесеттингс.|
|[Обновление Привилежедролесеттингс](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Обновление объекта Привилежедролесеттингс.|
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|елеватиондуратион|duration|Продолжительность активации роли.|
|id|string| Уникальный идентификатор для параметров роли. Только для чтения.|
|исмфаонелеватионконфигурабле|boolean|**значение true** , если мфаонелеватион является настраиваемым. **false** , если мфаонелеватион не является настраиваемым.|
|ластглобаладмин|boolean|Только для внутреннего использования.|
|макселаватиондуратион|duration|Максимальный срок для активированной роли.|
|мфаонелеватион|boolean|**значение true** , если для активации роли требуется mfa. **false** , если MFA не требуется для активации роли.|
|минелеватиондуратион|duration|Минимальная длительность для активированной роли.|
|нотификатионтаусеронелеватион|boolean|**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли. **значение false** , если уведомление не отправляется при активации роли.|
|тиккетингинфунелеватион|boolean|**имеет значение true** , если при активации роли требуются сведения о билетах. **false** , если при активации роли не требуются сведения о билетах.|
|аппровалонелеватион|boolean|**имеет значение true** , если при активации роли необходимо выполнить утверждение. **false** , если при активации роли не нужно утверждать.|
|аппроверидс| Коллекция строк |Список идентификаторов утверждения, если для активации необходимо утверждение.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
