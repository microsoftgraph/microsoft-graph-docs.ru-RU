---
title: Получение Пассвордаусентикатионмесод
description: Получение свойств и связей объекта пассвордаусентикатионмесод.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c11a59c4c63aa27df759e462fbc0f7fdea7c2c8
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806523"
---
# <a name="get-passwordauthenticationmethod"></a>Получение Пассвордаусентикатионмесод

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств и связей объекта [метода проверки подлинности](../resources/passwordauthenticationmethod.md) с помощью пароля. 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения, действующие на себя (по крайней мере для самых привилегированных) | Разрешения, действующие на других (по крайней мере для самых привилегированных)|
|:---------------------------------------|:-------------------------|:-----------------|
| Делегированные (рабочая или учебная учетная запись)     | Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL | Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. | Не поддерживается. |
| Для приложений                            | Не поддерживается. | Не поддерживается. |

Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* Глобальный администратор
* Глобальный читатель
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [пассвордаусентикатионмесод](../resources/passwordauthenticationmethod.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "28c10230-6103-485e-b985-444c60001490",
  "password": null,
  "creationDateTime": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get passwordAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
