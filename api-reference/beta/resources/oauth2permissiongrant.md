---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет делегированные разрешения (области OAuth 2.0), которые были предоставлены приложению, часто в результате процесса предоставления согласия пользователя или администратора.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: c8c0c0596246b1267d5cec619928d9d4fc9a13bf
ms.sourcegitcommit: 191b797b178f40fde6419719fcd75461e6869401
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2022
ms.locfileid: "66118622"
---
# <a name="oauth2permissiongrant-resource-type"></a>Тип ресурса oAuth2PermissionGrant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет делегированные разрешения, предоставленные субъекту-службе приложения.

Делегированные разрешения можно создать в результате предоставления пользователем запроса приложения на доступ к API или создания напрямую.

Делегированные разрешения иногда называют "областями OAuth 2.0" или "областями".

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Перечисление oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md) | Получение списка делегированных разрешений. |
| [Получение oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)  | Чтение одного делегированного разрешения.|
| [Создание oAuth2PermissionGrant](../api/oauth2permissiongrant-post.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) | Создайте делегированное предоставление разрешений. |
| [Обновление oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | Нет | Обновление объекта oAuth2PermissionGrant. |
| [Удаление oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | Нет  | Удаление делегированного разрешения. |
| [Delta](../api/oauth2permissiongrant-delta.md) | Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md) |Получение вновь созданных, обновленных или удаленных объектов **oauth2permissiongrant** без выполнения полного чтения всей коллекции ресурсов. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| id | Строка | Уникальный идентификатор **объекта oAuth2PermissionGrant**. Только для чтения.|
| clientId | String | Идентификатор **субъекта-службы** клиента для приложения, которому разрешено действовать от имени вошедвшего пользователя при доступе к API.[](serviceprincipal.md) Обязательный аргумент. Поддерживает `$filter` (только `eq`). |
| consentType | Строка | Указывает, предоставляется ли клиентское приложение авторизации для олицетворения всех пользователей или только определенного пользователя. *AllPrincipals* указывает авторизацию для олицетворения всех пользователей. *Субъект* указывает авторизацию для олицетворения определенного пользователя. Согласие от имени всех пользователей может предоставить администратор. В некоторых случаях пользователи, не являемые администраторами, могут иметь разрешение на предоставление согласия от имени себя для некоторых делегированных разрешений. Обязательный аргумент. Поддерживает `$filter` (только `eq`). |
| principalId | Строка | Идентификатор **пользователя,** от имени [](user.md) которого клиент имеет право на доступ к ресурсу, если **consentType** имеет значение *Principal*. Если **consentType** имеет *значение AllPrincipals* , это значение равно NULL. Требуется, если **consentType является principal***.* Поддерживает `$filter` (только `eq`). |
| resourceId | String | Идентификатор **субъекта-службы** [ресурсов](serviceprincipal.md) , к которому авторизован доступ. Это определяет API, клиент которого имеет право на попытку вызова от имени вошедвшего пользователя. Поддерживает `$filter` (только `eq`). |
| scope | String | Разделенный пробелами список значений утверждений для делегированных разрешений, которые должны быть включены в маркеры доступа для приложения ресурсов (API). Например, `openid User.Read GroupMember.Read.All`. Каждое значение утверждения должно соответствовать полю значения одного из делегированных разрешений, определенных API, перечисленным в свойстве **publishedPermissionScopes**  субъекта-службы [ресурсов](serviceprincipal.md). |
| startTime | DateTimeOffset | В настоящее время значение времени начала игнорируется, но при создании **объекта oAuth2PermissionGrant требуется значение**. Обязательный аргумент. |
| истечение срока действия | DateTimeOffset | В настоящее время значение конечного времени игнорируется, но при создании **объекта oAuth2PermissionGrant требуется значение**. Обязательный. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

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
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)",
  "expiryTime": "String (timestamp)"
}
```

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


