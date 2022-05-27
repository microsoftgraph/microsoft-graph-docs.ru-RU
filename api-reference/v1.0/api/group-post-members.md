---
title: Добавление участников
description: Добавляйте участника в группу Microsoft 365 или группу безопасности через свойство навигации members.
ms.localizationpriority: high
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2a3367ac195ee2bd252c32d83aa2dfd43c36d030
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694757"
---
# <a name="add-members"></a>Добавление участников

Пространство имен: microsoft.graph

Добавляйте участника в группу Microsoft 365 или группу безопасности через свойство навигации **members**.

В следующей таблице показаны типы участников, которых можно добавить в группы безопасности или группы Microsoft 365.

| Тип объектов             | Участник групп безопасности.     | Участник группы Microsoft 365 |
|-------------------------|-------------------------------|-------------------------------|
| Пользователи                   | ![Может быть участником группы][Yes]   | ![Может быть участником группы][Yes]   |
| Группы безопасности         | ![Может быть участником группы][Yes]   | ![Не может быть участником группы][No] |
| Группах Microsoft 365    | ![Не может быть участником группы][No] | ![Не может быть участником группы][No] |
| Устройства                 | ![Может быть участником группы][Yes]   | ![Не может быть участником группы][No] |
| Субъекты-службы      | ![Может быть участником группы][Yes]   | ![Не может быть участником группы][No] |
| Контакты организации | ![Может быть участником группы][Yes]   | ![Не может быть участником группы][No] |

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                |
| :------------------------------------- | :------------------------------------------------------------------------- |
| Делегированное (рабочая или учебная учетная запись)     | GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All    |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                                                             |
| Для приложения                            | GroupMember.ReadWrite.All, Group.ReadWrite.All и Directory.ReadWrite.All |

> [!IMPORTANT]
> Чтобы добавить участников в группу с возможностью назначения ролей, необходимо также назначить разрешение _RoleManagement.ReadWrite.Directory_ вызывающему пользователю или приложению.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                       |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Основной текст запроса

Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) или [organizational contact](../resources/orgcontact.md) в формате JSON.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика. Если объект уже является членом группы, этот метод возвращает код отклика `400 Bad Request`. Если добавляемый объект не существует, этот метод возвращает код отклика `404 Not Found`.

## <a name="examples"></a>Примеры

### <a name="example-1-add-a-member-to-a-group"></a>Пример 1. Добавление участника группы

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "add_member_to_group"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{group-id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-member-to-group-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/add-member-to-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/add-member-to-group-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/add-member-to-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

Укажите в тексте запроса свойство добавляемого объекта идентификатор directoryObject, user или group, представленное в формате JSON.

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a>Пример 2. Добавление нескольких участников в группу одним запросом

В этом примере показано, как добавить нескольких участников в группу с поддержкой с привязкой к ОData в операции PATCH. Обратите внимание, что одним запросом можно добавить до 20 участников. Операция POST не поддерживается. Если в тексте запроса существует условие ошибки, элементы не добавляются и возвращается соответствующий код отклика.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "add_multiple_members_to_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{group-id}
Content-type: application/json

{
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-multiple-members-to-group-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/add-multiple-members-to-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/add-multiple-members-to-group-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/add-multiple-members-to-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

Укажите в тексте запроса свойство добавляемого объекта идентификатор directoryObject, user или group, представленное в формате JSON.

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

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



[Yes]: /graph/images/yesandnosymbols/greencheck.svg
[No]: /graph/images/yesandnosymbols/no.svg

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api/group-post-members.md:
      Failed to parse enumeration values for type microsoft.graph.add. Table requires a column header named one of the following: Member, Name, Value"
  ]
}-->
