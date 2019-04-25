---
title: Тип ресурса Привилежедролесеттингс
description: Представляет параметры привилегированной роли.
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563287"
---
# <a name="privilegedrolesettings-resource-type"></a>Тип ресурса Привилежедролесеттингс

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
|Елеватиондуратион|duration|Продолжительность активации роли.|
|id|string| Уникальный идентификатор для параметров роли. Только для чтения.|
|Исмфаонелеватионконфигурабле|boolean|**значение true** , если мфаонелеватион является настраиваемым. **false** , если мфаонелеватион не является настраиваемым.|
|Ластглобаладмин|boolean|Только для внутреннего использования.|
|Макселаватиондуратион|duration|Максимальный срок для активированной роли.|
|Мфаонелеватион|boolean|**значение true** , если для активации роли требуется mfa. **false** , если MFA не требуется для активации роли.|
|Минелеватиондуратион|duration|Минимальная длительность для активированной роли.|
|Нотификатионтаусеронелеватион|boolean|**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли. **значение false** , если уведомление не отправляется при активации роли.|
|Тиккетингинфунелеватион|boolean|**имеет значение true** , если при активации роли требуются сведения о билетах. **false** , если при активации роли не требуются сведения о билетах.|
|Аппровалонелеватион|boolean|**имеет значение true** , если при активации роли необходимо выполнить утверждение. **false** , если при активации роли не нужно утверждать.|
|Аппроверидс|массив|Список идентификаторов утверждения, если для активации необходимо утверждение.|

## <a name="relationships"></a>Отношения
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
