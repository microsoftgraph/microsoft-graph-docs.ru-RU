---
title: 'user: translateExchangeIds'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 030594006de62bb4c146cad4cae70fcb4c51485c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176397"
---
# <a name="user-translateexchangeids"></a>user: translateExchangeIds

Пространство имен: microsoft.graph

Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | User.ReadBasic.All, User.Read, User.ReadWrite |
| Для приложений | User.Read.All, User.ReadWrite.All |

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

| Параметр | Тип | Описание |
|:----------|:-----|:------------|
| inputIds | Коллекция объектов string | Коллекция идентификаторов для преобразования. Все идентификаторы в коллекции ДОЛЖНЫ иметь одинаковый тип идентификатора источника и должны быть для элементов в одном почтовом ящике. Максимальный размер этой коллекции составляет 1000 строк. |
| sourceIdType | exchangeIdFormat | Тип идентификаторов в `InputIds` параметре. |
| targetIdType | exchangeIdFormat | Запрашиваемого типа ID для преобразования. |

### <a name="exchangeidformat-values"></a>Значения exchangeIdFormat

| Member | Описание |
|:-------|:------------|
| entryId | Формат двоичных записей, используемый клиентами MAPI. |
| ewsId | Формат ИД, используемый клиентами веб-служб Exchange. |
| immutableEntryId | Двоичный формат ID, совместимый с MAPI. |
| restId | Формат по умолчанию, используемый Microsoft Graph. |
| restImmutableEntryId | Не изменяемый формат ИД, используемый в Microsoft Graph. |

Двоичные форматы `entryId` `immutableEntryId` (и) — это безопасный URL-адрес в коде base64. Защита URL-адресов реализуется путем изменения кодировидности base64 двоичных данных следующим образом:

- Заменить `+` на `-`
- Заменить `/` на `_`
- Удалите все символы заполнения в окнах ( `=` )
- Добавьте в конец строки integer, указывающее, сколько символов заполнения было в исходном ( `0` , , , или `1` `2` )

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает `200 OK` код отклика и [коллекцию convertIdResult](../resources/convertidresult.md) в тексте отклика.

## <a name="example"></a>Пример

В следующем примере показано, как преобразовать несколько идентификаторов из обычного формата REST API ( ) в `restId` необраменяемый формат REST ( `restImmutableEntryId` ).

### <a name="request"></a>Запрос

Ниже представлен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/translateExchangeIds
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-translateexchangeids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Вот пример ответа
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```

