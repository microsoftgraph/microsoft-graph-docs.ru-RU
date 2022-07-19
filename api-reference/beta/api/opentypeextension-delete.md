---
title: Удаление openTypeExtension
description: 'Удаление открытого расширения (объекта openTypeExtension) из указанного экземпляра ресурса. '
ms.localizationpriority: medium
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: d41d6e784c5e2194bc2a4671ace11f44f56ac529
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855751"
---
# <a name="delete-opentypeextension"></a>Удаление openTypeExtension

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

Удаление открытого расширения (объекта [openTypeExtension](../resources/opentypeextension.md)) из указанного экземпляра ресурса. 

Список ресурсов, поддерживающих [открытые](#permissions) расширения, см. в таблице в разделе "Разрешения".

## <a name="permissions"></a>Разрешения

В зависимости от ресурса, из который вы удаляете расширение, и запрашиваемого типа разрешений (делегированного или приложения), разрешение, указанное в следующей таблице, является наименее привилегированным, необходимым для вызова этого API. Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Приложение |
|:-----|:-----|:-----|:-----|
| [baseTask](../resources/basetask.md) (не рекомендуется) | Tasks.ReadWrite | Tasks.ReadWrite | Tasks.ReadWrite.All |
| [baseTasklist](../resources/basetasklist.md) (не рекомендуется) | Tasks.ReadWrite | Tasks.ReadWrite | Tasks.ReadWrite.All |
| [device](../resources/device.md) | Directory.AccessAsUser.All | Не поддерживается | Device.ReadWrite.All |
| [event](../resources/event.md) | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| [group](../resources/group.md) | Group.ReadWrite.All | Не поддерживается | Group.ReadWrite.All |
| [event](../resources/event.md) для групп | Group.ReadWrite.All | Не поддерживается | Не поддерживается |
| [post](../resources/post.md) для групп | Group.ReadWrite.All | Не поддерживается | Group.ReadWrite.All |
| [message](../resources/message.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite | 
| [organization](../resources/organization.md) | Organization.ReadWrite.All | Не поддерживается | Organization.ReadWrite.All |
| [contact](../resources/contact.md) (личный контакт) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [todoTask](../resources/todotask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Tasks.ReadWrite.All |
| [todoTasklist](../resources/todotasklist.md)  | Tasks.ReadWrite | Tasks.ReadWrite | Tasks.ReadWrite.All |
| [user](../resources/user.md) | User.ReadWrite | User.ReadWrite | User.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

В запросе идентифицируйте экземпляр ресурса, воспользуйтесь свойством навигации **extensions** этого экземпляра, чтобы определить расширение, и укажите метод `DELETE` для этого экземпляра расширения.

<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{administrativeUnitId}/extensions/{extensionId}
DELETE /devices/{deviceId}/extensions/{extensionId}
DELETE /users/{userId|userPrincipalName}/events/{eventId}/extensions/{extensionId}
DELETE /groups/{groupId}/extensions/{extensionId}
DELETE /groups/{groupId}/events/{eventId}/extensions/{extensionId}
DELETE /groups/{groupId}/threads/{threadIid}/posts/{postId}/extensions/{extensionId}
DELETE /users/{userIid|userPrincipalName}/messages/{messageId}/extensions/{extensionId}
DELETE /organization/{organizationId}/extensions/{extensionId}
DELETE /users/{userId|userPrincipalName}/contacts/{contactId}/extensions/{extensionId}
DELETE /users/{userId|userPrincipalName}/extensions/{extensionId}
DELETE /users/me/todo/lists/{listId}/extensions/{extensionId}
DELETE /users/me/todo/lists/{listId}/tasks/{taskId}/extensions/{extensionId}
DELETE /users/me/tasks/lists/{listId}/extensions/{extensionId}
DELETE /users/me/tasks/lists/{listId}/tasks/{taskId}/extensions/{extensionId}
```

>**Примечание.** В приведенном выше синтаксисе показаны некоторые распространенные способы определения экземпляра ресурса, чье расширение нужно удалить. Все другие варианты синтаксиса, позволяющие определить эти экземпляры ресурса, поддерживают удаление открытых расширений этих экземпляров подобным образом.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Значение |
|:---------------|:----------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В первом примере показано, как сослаться на расширение по его имени и удалить расширение в указанном сообщении.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-opentypeextension-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-opentypeextension-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Во втором примере показано, как удалить расширение в событии указанной группы.

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


