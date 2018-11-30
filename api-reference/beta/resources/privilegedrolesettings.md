---
title: Тип ресурса privilegedRoleSettings
description: Представляет параметры для привилегированной роли.
ms.openlocfilehash: 14b4919d653de80c97f06aff507c011162c3c0e4
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2018
ms.locfileid: "27082893"
---
# <a name="privilegedrolesettings-resource-type"></a>Тип ресурса privilegedRoleSettings

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет параметры для привилегированной роли.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Чтение свойства и связи объекта privilegedRoleSettings.|
|[Обновление privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Обновление объекта privilegedRoleSettings.|
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|elevationDuration|duration|Длительность, при активации роли.|
|id|строка| Уникальный идентификатор для параметров роли. Только для чтения.|
|isMfaOnElevationConfigurable|boolean|**значение true,** Если mfaOnElevation может быть настроен. **значение false,** Если mfaOnElevation не настраивается.|
|lastGlobalAdmin|boolean|Для внутреннего использования используется только.|
|maxElavationDuration|duration|Максимальной длительности для активации роли.|
|mfaOnElevation|boolean|**значение true,** Если необходимо активировать роль многофакторной проверкой Подлинности. **значение false,** Если многофакторной проверкой Подлинности не требуется для включения роли.|
|minElevationDuration|duration|Минимальная продолжительность активированные роли.|
|notificationToUserOnElevation|boolean|**значение true,** Если отправить уведомление конечному пользователю при активации роли. **значение false,** Если не отправлять уведомления при активации роли.|
|ticketingInfoOnElevation|boolean|**значение true,** Если отдела сведения требуется при активации роли. **значение false,** Если отдела сведения не является обязательным, когда активировать роль.|
|approvalOnElevation|boolean|**значение true,** Если требуется утверждение при активации роли. **значение false,** Если утверждение не является обязательным, когда активировать роль.|
|approverIds|array|Список идентификаторов утверждения, если требуется для активации утверждение.|

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
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->