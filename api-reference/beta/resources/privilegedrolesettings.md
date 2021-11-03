---
title: тип ресурса privilegedRoleSettings
description: Представляет параметры привилегированной роли.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 6085d6bc74a1399ea4baf0cc575ecb316a3519e9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694169"
---
# <a name="privilegedrolesettings-resource-type"></a>тип ресурса privilegedRoleSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры привилегированной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Чтение свойств и связей объекта privilegedRoleSettings.|
|[Обновление privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Обновление объекта privilegedRoleSettings.|
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|elevationDuration|duration|Продолжительность активации роли.|
|id|string| Уникальный идентификатор параметров ролей. Только для чтения.|
|isMfaOnElevationConfigurable|логический|`true` если **mfaOnElevation** настраивается. `false` если **mfaOnElevation** не настраивается.|
|lastGlobalAdmin|логический|Только для внутреннего использования.|
|maxElavationDuration|duration|Максимальная продолжительность для активированной роли.|
|mfaOnElevation|логический|`true` если для активации роли требуется MFA. `false` если MFA не требуется активировать роль.|
|minElevationDuration|duration|Минимальная продолжительность для активированной роли.|
|notificationToUserOnElevation|логический|`true` при отправке уведомления конечному пользователю при активации роли. `false` если не отправлять уведомления при активации роли.|
|ticketingInfoOnElevation|логический|`true` если при активации роли требуется информация о билетах. `false` если сведения о билетах не требуются при активации роли.|
|approvalOnElevation|логический|`true` если требуется утверждение при активации роли. `false` если утверждение не требуется при активации роли.|
|approverIds| string collection |Список ids утверждения, если требуется утверждение для активации.|

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


