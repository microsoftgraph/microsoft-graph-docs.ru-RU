---
title: Список участников роли каталога
description: Извлечение списка директоров, которые назначены роли каталога.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a503fe928f4b06fd728d9425fafdb9cf8fc1f8c9
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672534"
---
# <a name="list-members-of-a-directory-role"></a>Список участников роли каталога

Пространство имен: microsoft.graph

Извлечение списка директоров, которые назначены роли каталога. 

С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole** . ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure. Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-id}/members
GET /directoryRoles/roleTemplateId={roleTemplateId}/members
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.
## <a name="examples"></a>Примеры

### <a name="example-1-get-the-members-of-a-directory-role-using-role-id"></a>Пример 1. Получить членов роли каталога с помощью id роли

#### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_objectid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryrole-members-objectid-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-directoryrole-members-objectid-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик
> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```
### <a name="example-2-get-the-members-of-a-directory-role-using-roletemplateid"></a>Пример 2. Получить членов роли каталога с помощью roleTemplateId

### <a name="request"></a>Запрос

<!-- disabling snippet generation because of an SDK limitation. For more information, see https://github.com/microsoftgraph/msgraph-sdk-dotnet/issues/1041-->

<!-- {
  "blockType": "ignored",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
