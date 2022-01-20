---
title: Добавление участников
description: Добавляйте участника в группу Microsoft 365 или группу безопасности через свойство навигации members.
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ad454155b471eee5338c1efffc670a56dc820689
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113392"
---
# <a name="add-members"></a>Добавление участников

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавляйте участника в группу Microsoft 365 или группу безопасности через свойство навигации **members**.

Можно добавить пользователей, директоров служб или другие группы. 

> [!IMPORTANT]
> + Можно добавить участников только в группы безопасности и Microsoft 365.
> + Вы не можете добавлять группы безопасности в группы Microsoft 365.
> + Вы не можете добавлять группы Microsoft 365 в группы безопасности или другие группы Microsoft 365.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a>Заголовки запросов
| Имя | Описание|
|:---- |:-----------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика. Если объект уже является членом группы, этот метод возвращает код отклика `400 Bad Request`. Если добавляемый объект не существует, этот метод возвращает код отклика `404 Not Found`. 

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{group-id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-group-member-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/add-group-member-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

В теле запроса устройте JSON-представление объекта `id` [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или группового объекта, который необходимо добавить. [](../resources/group.md)

### <a name="response"></a>Отклик
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
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


