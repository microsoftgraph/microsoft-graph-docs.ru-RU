---
title: Предоставление appRoleAssignment субъекту-службе
description: Предоставляйте назначение роли приложения субъекту-службе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: bda33fd1ae7fed99bf440f604208a7eef3afabf7
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667796"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a>Предоставление appRoleAssignment субъекту-службе

Пространство имен: microsoft.graph

Назначение роли приложения для этого субъекта-службы пользователю, группе или субъекту-службе клиента.

Роли приложений, назначаемые субъектам-службам, также называются [разрешениями приложений](/azure/active-directory/develop/v2-permissions-and-consent#permission-types). Разрешения приложений можно предоставлять непосредственно в назначениях ролей приложений, а также с помощью [интерфейса согласия](/azure/active-directory/develop/application-consent-experience).

Чтобы предоставить назначение роли приложения, нужны три идентификатора:

- `principalId`: `id` **пользователя**, **группы** или объекта **servicePrincipal** клиента, которому назначается роль приложения.
- `resourceId`: `id` ресурса **servicePrincipal**, определяющий роль приложения.
- `appRoleId`: `id` объекта **appRole** (определенного в субъекте-службе ресурса) для назначения пользователю, группе или субъекту-службе.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AppRoleAssignment.ReadWrite.All и Application.Read.All, AppRoleAssignment.ReadWrite.All и Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.AllAll    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | AppRoleAssignment.ReadWrite.All и Application.Read.All, AppRoleAssignment.ReadWrite.All и Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

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
  "name": "serviceprincipal_create_approleassignedto"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignedTo
Content-Type: application/json

{
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В этом примере `{id}` и `{resourceId-value}` оба будут `id` субъекта-службы ресурса, а `{principalId}` будет `id` назначенного пользователя, группы или субъекта-службы клиента.

### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('9028d19c-26a9-4809-8e3f-20ff73e2d75e')/appRoleAssignedTo/$entity",
  "id": "-WmtM5na7Uus0D8kI1yylpU9Mdo0Pb9OoBJvd3T5eKc",
  "deletedDateTime": null,
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7",
  "createdDateTime": "2021-02-15T16:14:59.8643039Z",
  "principalDisplayName": "Parents of Contoso",
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "principalType": "Group",
  "resourceDisplayName": "Fabrikam App",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
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
