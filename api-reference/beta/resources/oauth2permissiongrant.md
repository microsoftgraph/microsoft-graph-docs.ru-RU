---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет области OAuth 2.0 (делегированы разрешения), которые были присвоены приложения (представленного участников-служб) в ходе процесса согласия пользователь или администратор.
ms.openlocfilehash: 8fc5154ddba1b78976dc3e24c6712f9fc8944f43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076014"
---
# <a name="oauth2permissiongrant-resource-type"></a>Тип ресурса oAuth2PermissionGrant

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет области OAuth 2.0 (делегированы разрешения), которые были присвоены приложения (представленного участников-служб) в ходе процесса согласия пользователь или администратор.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
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
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|clientId|String| Идентификатор участника службы предоставляются разрешения для олицетворения пользователя при доступе к ресурсу, (представлено свойством Ид_ресурса). |
|consentType|String| Указывает, если согласие предоставленный администратором (от имени организации) или пользователем. Возможные значения: *AllPrincipals* или *участника*. |
|expiryTime|DateTimeOffset| На данный момент игнорируется значение времени истечения срока действия. |
|id|String| Уникальный идентификатор. Только для чтения.|
|principalId|String| Если consentType является *AllPrincipals* это значение равно null и согласия применяется ко всем пользователям в организации. Если consentType является *основной*, это свойство определяет идентификатор пользователя, который предоставлены разрешения и применяется только к этому пользователю. |
|resourceId|String| Задает идентификатор участника службы ресурсов, к которому был разрешен доступ. |
|scope|String| Задает значение утверждения [область](/graph/permissions-reference) , должно привести к приложению ресурсов в маркер доступа OAuth 2.0. Например, *User.Read* |
|startTime|DateTimeOffset| На данный момент времени начала игнорируется. |

## <a name="relationships"></a>Связи
Нет


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Чтение свойства и связи объекта oAuth2PermissionGrant.|
|[Список oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) коллекции | Получение списка объектов oauth2PermissionGrant. |
|[Обновление oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Обновление объекта oAuth2PermissionGrant. |
|[Удаление oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Нет |Удалите объект oAuth2PermissionGrant. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->