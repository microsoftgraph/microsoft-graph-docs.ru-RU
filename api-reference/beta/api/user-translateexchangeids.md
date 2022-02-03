---
title: 'пользователь: translateExchangeIds'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: abheek-das
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 20fac290ea2baf68b2780e75224724616a2814c3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341025"
---
# <a name="user-translateexchangeids"></a>пользователь: translateExchangeIds

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

| Параметр | Тип | Описание |
|:----------|:-----|:------------|
| inputIds | Коллекция String | Коллекция идентификаторов для преобразования. Все идентификаторы в коллекции должны иметь один и тот же тип идентификатора источника и должны быть для элементов в одном почтовом ящике. Максимальный размер этой коллекции — 1000 строк. |
| sourceIdType | exchangeIdFormat | Идентификатор идентификаторов в параметре `InputIds` . |
| targetIdType | exchangeIdFormat | Запрашиваемого типа ID для преобразования. |

### <a name="exchangeidformat-values"></a>Значения exchangeIdFormat

| Member | Описание |
|:-------|:------------|
| entryId | Двоичный формат входа, используемый клиентами MAPI. |
| ewsId | Формат ID, используемый Exchange веб-службами. |
| immutableEntryId | Двоичный формат ID, совместимый с MAPI. |
| restId | Формат ID по умолчанию, используемый Корпорацией Майкрософт Graph. |
| restImmutableEntryId | Неоменяемый формат ID, используемый Корпорацией Майкрософт Graph. |

Двоичные форматы (`entryId` и `immutableEntryId`) — это кодируемые URL-адреса base64. Безопасность URL-адресов реализуется путем изменения кодирования двоичных данных base64 следующим образом:

- Замените `+` на `-`
- Замените `/` на `_`
- Удалите любые символы обивки с прицепом (`=`)
- Добавьте в конец строки integer, указывающее, сколько символов обивки было в оригинале (`0`или`1``2`)

## <a name="response"></a>Отклик

В случае успешной работы этот `200 OK` метод возвращает код отклика и [коллекцию convertIdResult](../resources/convertidresult.md) в тексте ответа.

## <a name="example"></a>Пример

В следующем примере показано, как преобразовать несколько идентификаторов из обычного формата API REST (`restId`) в неоменяемый формат REST (`restImmutableEntryId`).

### <a name="request"></a>Запрос

Ниже представлен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-translateexchangeids-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-translateexchangeids-powershell-snippets.md)]
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


