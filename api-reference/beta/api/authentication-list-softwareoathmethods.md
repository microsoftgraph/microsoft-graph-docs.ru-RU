---
title: Список softwareOathMethods
description: Извлечение списка объектов программного обеспечения пользователяOathAuthenticationMethods и их свойств.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7fc0bf9d2a834c9ffb01cbe23ae2d3adb009fd3b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995236"
---
# <a name="list-softwareoathmethods"></a>Список softwareOathMethods
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка объектов метода проверки подлинности маркеров с помощью программного обеспечения [OATH](../resources/softwareoathauthenticationmethod.md) и их свойств.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-acting-on-self"></a>Разрешения, действующие на себя

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

### <a name="permissions-acting-on-other-users"></a>Разрешения, действующие на других пользователей

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All |

Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих ролей [каталога:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)
* Глобальный читатель
* администратор проверки подлинности.
* привилегированный администратор проверки подлинности;
* Глобальный администратор

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/softwareOathMethods
GET /users/{id | userPrincipalName}/authentication/softwareOathMethods
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [softwareOathAuthenticationMethod](../resources/softwareoathauthenticationmethod.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_softwareoathauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/softwareOathMethods
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-softwareoathauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-softwareoathauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-softwareoathauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-softwareoathauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-softwareoathauthenticationmethod-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.softwareOathAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.softwareOathAuthenticationMethod",
      "id": "b172893e-893e-b172-3e89-72b13e8972b1",
      "secretKey": "String"
    }
  ]
}
```
