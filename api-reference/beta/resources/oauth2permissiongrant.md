---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.
localization_priority: Normal
ms.openlocfilehash: f23d2e7a8b57b324a92a1268ab4cc0393d8906f0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342074"
---
# <a name="oauth2permissiongrant-resource-type"></a>Тип ресурса oAuth2PermissionGrant

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|clientId|String| Идентификатор субъекта-службы, которому предоставлено согласие на олицетворение пользователя при доступе к ресурсу (представленному свойством resourceId). |
|Консенттипе|String| Указывает, было ли согласие предоставлено администратором (от имени Организации) или отдельным пользователем. Возможные значения: *аллпринЦипалс* или *Principal*. |
|Експиритиме|DateTimeOffset| В настоящее время значение срока действия игнорируется. |
|id|Строка| Уникальный идентификатор. Только для чтения.|
|principalId|String| Если Консенттипе — *аллпринЦипалс* , это значение равно null, а согласие применяется ко всем пользователям в Организации. Если Консенттипе является *субъектом*, это свойство указывает идентификатор пользователя, который предоставил согласие и применяется только для этого пользователя. |
|resourceId|String| Указывает идентификатор субъекта службы ресурсов, которому предоставлен доступ. |
|scope|String| Указывает значение утверждения [области](/graph/permissions-reference) , которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0. Например, *User. Read* |
|startTime|DateTimeOffset| В настоящее время значение времени начала игнорируется. |

## <a name="relationships"></a>Связи
Нет


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Чтение свойств и связей объекта oAuth2PermissionGrant.|
|[Список oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md) | Получение списка объектов oauth2PermissionGrant. |
|[Обновление oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Обновление объекта oAuth2PermissionGrant. |
|[Удаление oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Нет |Удаление объекта oAuth2PermissionGrant. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
