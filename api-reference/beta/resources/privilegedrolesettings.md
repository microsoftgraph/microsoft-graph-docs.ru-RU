---
title: Тип ресурса privilegedRoleSettings
description: Представляет параметры привилегированной роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: efc04b9b65719cbd5952dffb545d371172ab95eb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137636"
---
# <a name="privilegedrolesettings-resource-type"></a>Тип ресурса privilegedRoleSettings

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
|id|string| Уникальный идентификатор для параметров роли. Только для чтения.|
|isMfaOnElevationConfigurable|boolean|**true,** если mfaOnElevation настраивается. **false,** если mfaOnElevation не настраивается.|
|lastGlobalAdmin|boolean|Только для внутреннего использования.|
|maxElavationDuration|duration|Максимальная длительность активированной роли.|
|mfaOnElevation|boolean|**имеет значение true,** если для активации роли требуется многофаксная активация. **false,** если MFA не требуется для активации роли.|
|minElevationDuration|duration|Минимальная длительность активированной роли.|
|notificationToUserOnElevation|boolean|имеет значение **true,** если при активации роли пользователю отправляется уведомление. **false,** если не отправлять уведомление при активации роли.|
|ticketingInfoOnElevation|boolean|имеет значение **true,** если при активации роли требуются сведения о билетах. **false,** если сведения о билетах не требуются при активации роли.|
|approvalOnElevation|boolean|имеет значение **true,** если требуется утверждение при активации роли. **false,** если утверждение не требуется при активации роли.|
|approverIds| Коллекция строк |Список ид утверждения, если для активации требуется утверждение.|

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


