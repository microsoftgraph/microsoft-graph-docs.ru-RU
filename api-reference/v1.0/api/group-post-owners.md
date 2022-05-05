---
title: Добавление владельцев
description: Добавьте пользователя или субъект-службу к владельцам группы Microsoft 365 или группы безопасности. Владельцы — это группа пользователей или субъектов-служб, которым разрешено изменять объект группы.
ms.localizationpriority: high
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5c0d24b34abdcfeab7566e9c9381ebdb807faeb0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205966"
---
# <a name="add-owners"></a>Добавление владельцев

Пространство имен: microsoft.graph

Добавьте пользователя или субъект-службу к владельцам группы Microsoft 365 или группы безопасности. Владельцы — это группа пользователей или субъектов-служб, которым разрешено изменять объект группы.

> **Важно!** При обновлении владельцев группы и создании команды для группы может потребоваться до 2 часов для синхронизации владельцев с Microsoft Teams. Кроме того, если нужно, чтобы владелец мог вносить изменения в команду, например путем создания плана Планировщика, владельца также требуется добавить в качестве участника группы или команды.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)  |
| :------------------------------------- | :------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Group.ReadWrite.All, Directory.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                               |
| Для приложений                            | Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/owners/$ref
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) или [servicePrincipal](../resources/serviceprincipal.md) в формате JSON с **@odata.id**.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика. Если объект уже является членом группы, этот метод возвращает код отклика `400 Bad Request`. Если добавляемый объект не существует, этот метод возвращает код отклика `404 Not Found`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приводится пример запроса, который добавляет пользователя в качестве владельца группы.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_owner_from_group"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/owners/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/create-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/create-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/create-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/create-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-owner-from-group-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/create-owner-from-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)

[!INCLUDE [sample-code](../includes/snippets/powershell/create-owner-from-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

Предоставьте в тексте запроса описание добавляемого объекта [user](../resources/user.md) или [servicePrincipal](../resources/user.md) в формате JSON с **@odata.id**.

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>См. также

- [Добавление участника в команду](team-post-members.md)
- [Обновление роли участника в группе](team-update-members.md)
- [Удаление участника из чата](team-delete-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
