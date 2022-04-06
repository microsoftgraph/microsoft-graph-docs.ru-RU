---
title: Методы List
description: Извлечение списка объектов метода проверки подлинности.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8814d4bcb6b5ebee28cf19cbdcbe6b4f5889bfc0
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510424"
---
# <a name="list-methods"></a>Методы List

Пространство имен: microsoft.graph

Извлечение списка [объектов authenticationMethod](../resources/authenticationmethod.md) . Этот API возвращает только методы проверки подлинности, поддерживаемые в этой версии API. Обзор [API методов проверки подлинности Azure AD](../resources/authenticationmethods-overview.md) см. в списке поддерживаемых в настоящее время методов.

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
|:---------------------------------------|:-------------------------|:-----------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All |

Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих ролей [Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):
* Глобальный администратор
* Глобальный читатель
* привилегированный администратор проверки подлинности;
* Администратор проверки подлинности (видит только номера телефонов в масках)

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод не поддерживает необязательные параметры запроса для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и коллекцию объектов [authenticationMethod](../resources/authenticationmethod.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
    },
    {
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
