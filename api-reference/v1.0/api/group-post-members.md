---
title: Добавление участников
description: Добавляйте участника в группу Microsoft 365 или группу безопасности через свойство навигации members.
ms.localizationpriority: high
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 95be30a6148a31b32123d0761de283320388f937
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672149"
---
# <a name="add-members"></a>Добавление участников

Пространство имен: microsoft.graph

Добавляйте участника в группу Microsoft 365 или группу безопасности через свойство навигации **members**.

Вы можете добавлять пользователей, контакты организации, cубъект-службы или другие группы. 

> [!IMPORTANT]
> + Вы можете добавить участников только в группы безопасности и группы Microsoft 365. Дополнительные сведения см. в разделе [Только типы групп в Azure AD и Microsoft Graph](/graph/api/resources/groups-overview#group-types-in-azure-ad-and-microsoft-graph).
> + Вы не можете добавлять группы безопасности в группы Microsoft 365.
> + Вы не можете добавлять группы Microsoft 365 в группы безопасности или другие группы Microsoft 365.
> + Группа безопасности может содержать пользователей, устройства, группы или субъекты-службы в качестве участников, а группа Microsoft 365 может содержать в качестве участников только пользователей.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложения | GroupMember.ReadWrite.All, Group.ReadWrite.All и Directory.ReadWrite.All |

> [!IMPORTANT]
> Чтобы добавить участников в группу с возможностью назначения ролей, необходимо также назначить разрешение *RoleManagement.ReadWrite.Directory* вызывающему пользователю или приложению.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |
| Content-Type   | application/json. Обязательный. |

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
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-member-to-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
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
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-multiple-members-to-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

