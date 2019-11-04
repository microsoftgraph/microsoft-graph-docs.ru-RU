---
title: Обновление Усераккаунтинформатион
description: Обновление свойств объекта Усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 78d890a00916c72b8c48e5b41a1c84e1e2e2ffb8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938143"
---
# <a name="update-useraccountinformation"></a>Обновление усераккаунтинформатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [усераккаунтинформатион](../resources/useraccountinformation.md) в [профиле](../resources/profile.md)пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | User. ReadWrite, User. ReadWrite. ALL          |
| Делегированные (личная учетная запись Майкрософт) | User. ReadWrite, User. ReadWrite. ALL          |
| Для приложений                            | User.ReadWrite.All                          |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя           |Описание                 |
|:---------------|:---------------------------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type   | application/json. Обязательное |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство            | Тип                                    | Описание                                                                                    |
|:--------------------|:----------------------------------------|:-----------------------------------------------------------------------------------------------|
|ageGroup             |String                                   |Показывает группу возрастных пользователей. Допустимые `null`значения `minor`, `notAdult` и `adult`. Только для чтения. |
|countryCode          |Строка                                   |Содержит два символа countryCode, связанных с учетной записью "Пользователи".                       |
|преферредлангуажетаг |[localeInfo](../resources/localeinfo.md) |Содержит язык, который пользователь связал с учетной записью как предпочитаемый.                     |
|userPrincipalName    |String                                   |Имя участника-пользователя (UPN) пользователя, связанного с учетной записью.                          |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [усераккаунтинформатион](../resources/useraccountinformation.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/account/{id}
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update useraccountinformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
