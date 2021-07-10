---
title: Get fido2AuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e4b5d5602c99b4a0c637f00a9bb638d456e8a3fd
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350994"
---
# <a name="get-fido2authenticationmethod"></a>Get fido2AuthenticationMethod
Пространство имен: microsoft.graph

Извлечение единого объекта проверки подлинности [ключа безопасности FIDO2 пользователя.](../resources/fido2authenticationmethod.md)

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

Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)
* Глобальный администратор
* Глобальный читатель
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности (видит только номера телефонов в масках)

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods/{id}
GET /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и запрашиваемого `200 OK` [объекта fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

``` http
GET https://graph.microsoft.com/v1.0/me/authentication/fido2Methods/-2_GRUg2-HYz6_1YG4YRAQ2
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
  }
}
```

