---
title: 'пользователь: translateExchangeIds'
description: Переведите идентификаторы, связанные с Outlook ресурсов форматов.
ms.openlocfilehash: 0c6e74ad0bb9676f261ed0202757b1e036b09c85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079252"
---
# <a name="user-translateexchangeids"></a>пользователь: translateExchangeIds

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Переведите идентификаторы, связанные с Outlook ресурсов форматов.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | User.ReadBasic, User.Read, User.ReadWrite |
| Для приложения | User.Read.All, User.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a>Заголовки запросов

| Имя | Значение |
|:-----|:------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

| Параметр | Тип | Description |
|:----------|:-----|:------------|
| inputIds | Edm.String коллекции | Коллекция идентификаторов для преобразования. Все идентификаторы в коллекции должны иметь одного идентификатор типа и значения для элементов в тот же почтовый ящик. Максимальный размер семейства сайтов составляет 1 000 строк. |
| sourceIdType | exchangeIdFormat | Тип идентификатора идентификаторов в `InputIds` параметр. |
| targetIdType | exchangeIdFormat | Запрошенный тип идентификатора для преобразования. |

### <a name="exchangeidformat-values"></a>exchangeIdFormat значения

| Значения | Описание |
|:-------|:------------|
| Идентификатор записи | Формат идентификатора двоичные запись, используемого клиентами MAPI. |
| ewsId | Идентификатор формата, используемого клиентами веб-служб Exchange. |
| immutableEntryId | MAPI-совместимое постоянные идентификатор формата. |
| restId | По умолчанию идентификатор формата Microsoft Graph. |
| restImmutableEntryId | Постоянные идентификатор формата, используемого в Microsoft Graph. |

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и семейства [convertIdResult](../resources/meetingtimesuggestionsresult.md) в теле ответа.

## <a name="example"></a>Пример

Следующем примере показано, как преобразовать несколько идентификаторов из обычного формата API-Интерфейс REST (`restId`) в формат постоянные REST (`restImmutableEntryId`).

##### <a name="request"></a>Запрос

Ниже представлен пример запроса.
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```

##### <a name="response"></a>Ответ

Ниже приведен пример ответа
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
  "value": [
    {
      "sourceId": "{rest-formatted-id-1},
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2},
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```