---
title: Предоставление appRoleAssignment субъекту-службе
description: Предоставление назначения роли приложения субъекту-службе
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 0bf60d6c72030a7b33fa926b4b4f4f192be43f5a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024254"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a>Предоставление appRoleAssignment субъекту-службе

Пространство имен: microsoft.graph


Назначьте роль приложения субъекту-службе клиента.

Роли приложений, назначаемые субъектам-службам, также называются [разрешениями приложений](/azure/active-directory/develop/v2-permissions-and-consent#permission-types). Разрешения приложения можно предоставлять непосредственно в назначениях ролей приложений, а также с помощью [интерфейса согласия](/azure/active-directory/develop/application-consent-experience).

Чтобы предоставить назначение роли приложения субъекту-службе клиента, нужны три идентификатора:

- `principalId`: `id` субъекта-службы клиента, которой нужно назначить роль приложения.
- `resourceId`: `id` ресурса `servicePrincipal` (API), в которых определена роль приложения (разрешение приложения).
- `appRoleId`: `id` объекта `appRole` (определенного в субъекте-службе ресурса) для назначения субъекту-службе клиента.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> Рекомендуется создавать назначения ролей приложения, используя [`appRoleAssignedTo`отношение _ресурса_ субъекта-службы](serviceprincipal-post-approleassignedto.md) вместо `appRoleAssignments`отношения назначенного пользователя, группы или субъекта-службы.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация | Bearer {token}. Обязательный.  |
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
  "name": "serviceprincipal_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignments
Content-Type: application/json

{
  "principalId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "resourceId": "8fce32da-1246-437b-99cd-76d1d4677bd5",
  "appRoleId": "498476ce-e0fe-48b0-b801-37ba7e2685c6"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-create-approleassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В этом примере обратите внимание, что значение, используемое в качестве **ИД** субъекта службы в URL-адресе запроса (`9028d19c-26a9-4809-8e3f-20ff73e2d75e`), совпадает со свойством **principalId** в тексте. Значение **resourceId** является **ИД** для субъекта-службы ресурса (API).

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appRoleAssignments/$entity",
  "id": "2jLOj0YSe0OZzXbR1Gd71fDqFUrPM1xIgUfvWBHJ9n0",
  "createdDateTime": "2021-02-15T16:39:38.2975029Z",
  "appRoleId": "498476ce-e0fe-48b0-b801-37ba7e2685c6",
  "principalDisplayName": "Fabrikam App",
  "principalId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "principalType": "ServicePrincipal",
  "resourceDisplayName": "Microsoft Graph",
  "resourceId": "8fce32da-1246-437b-99cd-76d1d4677bd5"
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
