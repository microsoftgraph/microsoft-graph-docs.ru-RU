---
title: Тип ресурса privilegedRoleSettings
description: Представляет параметры для привилегированной роли.
localization_priority: Normal
ms.openlocfilehash: 673327e3c83a4111eb469ca48550836433dbdf0a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577153"
---
# <a name="privilegedrolesettings-resource-type"></a>Тип ресурса privilegedRoleSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры для привилегированной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Чтение свойства и связи объекта privilegedRoleSettings.|
|[Обновление privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Обновление объекта privilegedRoleSettings.|
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|elevationDuration| String (метка времени) |Длительность, при активации роли.|
|id| String (идентификатор)| Уникальный идентификатор для параметров роли. Только для чтения.|
|isMfaOnElevationConfigurable|boolean|**значение true,** Если mfaOnElevation может быть настроен. **значение false,** Если mfaOnElevation не настраивается.|
|lastGlobalAdmin|boolean|Для внутреннего использования используется только.|
|maxElavationDuration| String (идентификатор)| |Максимальной длительности для активации роли.|
|mfaOnElevation|boolean|**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности. **значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли.|
|minElevationDuration|String (идентификатор)||Минимальная продолжительность активированные роли.|
|notificationToUserOnElevation|boolean|**значение true,** Если отправить уведомление конечному пользователю при активации роли. **значение false,** Если не отправлять уведомления при активации роли.|
|ticketingInfoOnElevation|boolean|**значение true,** Если отдела сведения требуется при активации роли. **значение false,** Если отдела сведения не является обязательным, когда активировать роль.|
|approvalOnElevation|boolean|**значение true,** Если требуется утверждение при активации роли. **значение false,** Если утверждение не является обязательным, когда активировать роль.|
|approverIds| Коллекция String |Список идентификаторов утверждения, если требуется для активации утверждение.|

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
  "approverIds": [ "String (identifier)" ]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
