---
title: Предоставление appRoleAssignment пользователю
description: Предоставление назначения роли приложения пользователю.
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 68733ebdea60565e7e9320510cb490233f702f10
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469411"
---
# <a name="grant-an-approleassignment-to-a-user"></a>Предоставление appRoleAssignment пользователю

Пространство имен: microsoft.graph

Используйте этот API, чтобы назначить роль приложения пользователю. Чтобы предоставить назначение роли приложения пользователю, нужны три идентификатора:

- `principalId`: `id` пользователя, которому нужно назначить роль приложения.
- `resourceId`: `id` ресурса `servicePrincipal`, который определяет роль приложения.
- `appRoleId`: `id` объекта `appRole` (определенного в субъекте-службе ресурса) для назначения пользователю.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | AppRoleAssignment.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/appRoleAssignments
```

> [!NOTE]
> Рекомендуется создавать назначения ролей приложения, используя отношение `appRoleAssignedTo` _ресурса_ субъекта-службы вместо отношения `appRoleAssignments` назначенного пользователя, группы или субъекта-службы.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {токен}. Обязательный.  |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите представление JSON для объекта [appRoleAssignment](../resources/approleassignment.md).

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает в тексте отклика код отклика `201 Created` и объект [appRoleAssignment](../resources/approleassignment.md).

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/users/cde330e5-2150-4c11-9c5b-14bfdc948c79/appRoleAssignments
Content-Type: application/json

{
  "principalId": "cde330e5-2150-4c11-9c5b-14bfdc948c79",
  "resourceId": "8e881353-1735-45af-af21-ee1344582a4d",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В этом примере обратите внимание, что значение, используемое в качестве **ИД** пользователя в URL-адресе запроса (`cde330e5-2150-4c11-9c5b-14bfdc948c79`), совпадает со свойством **principalId** в тексте сообщения.

### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('cde330e5-2150-4c11-9c5b-14bfdc948c79')/appRoleAssignments/$entity",
  "id": "5TDjzVAhEUycWxS_3JSMeY-oHkjrWvBKi7aIZwYGQzg",
  "deletedDateTime": null,
  "appRoleId": "00000000-0000-0000-0000-000000000000",
  "createdDateTime": "2021-02-15T10:31:53.5164841Z",
  "principalDisplayName": "Megan Bowen",
  "principalId": "cde330e5-2150-4c11-9c5b-14bfdc948c79",
  "principalType": "User",
  "resourceDisplayName": "dxprovisioning-graphapi-client",
  "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

