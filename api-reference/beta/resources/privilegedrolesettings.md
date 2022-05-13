---
title: Тип ресурса privilegedRoleSettings
description: Представляет параметры привилегированной роли.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 6c91003b7aa0455c6dd56b374fb45c3664111be3
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397498"
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
|elevationDuration|duration|Длительность активации роли.|
|id|string| Уникальный идентификатор параметров роли. Только для чтения.|
|isMfaOnElevationConfigurable|логический|`true` Значение **mfaOnElevation** можно настроить. `false` Значение **mfaOnElevation** не настраивается.|
|lastGlobalAdmin|логический|Только для внутреннего использования.|
|maxElavationDuration|duration|Максимальная длительность активированной роли.|
|mfaOnElevation|логический|`true` Значение , если для активации роли требуется многофакторная проверка подлинности. `false` Значение , если MFA не требуется для активации роли.|
|minElevationDuration|duration|Минимальная длительность активированной роли.|
|notificationToUserOnElevation|логический|`true` Значение , если при активации роли пользователю отправляется уведомление. `false` Значение , если не отправлять уведомление при активации роли.|
|ticketingInfoOnElevation|логический|`true` Значение , если сведения о запросе требуются при активации роли. `false` Значение , если сведения о запросе не требуются при активации роли.|
|approvalOnElevation|логический|`true` Значение , если требуется утверждение при активации роли. `false` Значение , если утверждение не требуется при активации роли.|
|approverIds| string collection |Список идентификаторов утверждения, если для активации требуется утверждение.|

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


