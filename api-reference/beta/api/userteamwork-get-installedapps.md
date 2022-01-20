---
title: Получить установленное приложение для пользователя
description: Извлечение приложения, установленного в личном поле указанного пользователя.
author: AkJo
doc_type: apiPageType
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: 11b2bf4b1af4f117e25c0b88d2174d615bb073fb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095689"
---
# <a name="get-installed-app-for-user"></a>Получить установленное приложение для пользователя

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Извлечение приложения,](../resources/teamsappinstallation.md) установленного в личном поле указанного [пользователя.](../resources/user.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id | user-principal-name}/teamwork/installedApps/{app-installation-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и приложение [в](../resources/teamsappinstallation.md) тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-get-an-app-installed-for-the-specified-user"></a>Пример 1. Установить приложение для указанного пользователя

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-list-teamsapps-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-list-teamsapps-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_1",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
### <a name="example-2-get-the-names-and-other-details-of-the-app-installed-for-the-user"></a>Пример 2. Получить имена и другие сведения о приложении, установленном для пользователя

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_details_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=?$expand=teamsAppDefinition
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-details-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-details-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-details-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-details-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-list-teamsapps-details-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-list-teamsapps-details-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details_1",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('5b649834-7412-4cce-9e69-176e95a394f5')/installedApps(teamsAppDefinition())/$entity",
      "id": "NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=",
      "teamsAppDefinition": {
        "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk=",
        "teamsAppId": "a6b63365-31a4-4f43-92ec-710b71557af9",
        "displayName": "Power Apps",
        "version": "0.9"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User get teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
