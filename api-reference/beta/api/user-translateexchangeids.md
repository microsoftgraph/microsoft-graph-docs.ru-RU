---
title: 'Пользователь: Транслатиксчанжеидс'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1015ae12f5ecfd63b29efe38f7172321b06386ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33961231"
---
# <a name="user-translateexchangeids"></a>Пользователь: Транслатиксчанжеидс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | User. ReadBasic, User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | User. ReadBasic, User. Read, User. ReadWrite |
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

## <a name="request-body"></a>Тело запроса

| Параметр | Тип | Описание |
|:----------|:-----|:------------|
| Инпутидс | Коллекция строк | Коллекция идентификаторов для преобразования. Все идентификаторы в коллекции должны иметь одинаковый тип идентификатора источника и должны быть для элементов в одном почтовом ящике. Максимальный размер этой коллекции составляет 1000 строк. |
| Саурцеидтипе | Ексчанжеидформат | Тип идентификатора идентификаторов в `InputIds` параметре. |
| Таржетидтипе | Ексчанжеидформат | Запрошенный тип идентификатора для преобразования. |

### <a name="exchangeidformat-values"></a>значения Ексчанжеидформат

| Значения | Описание |
|:-------|:------------|
| Код | Формат идентификатора двоичной записи, используемый клиентами MAPI. |
| Евсид | Формат идентификатора, используемый клиентами веб-служб Exchange. |
| Иммутаблинтрид | Двоичный формат неизменяемого идентификатора, совместимый с MAPI. |
| Рестид | Формат идентификатора по умолчанию, используемый Microsoft Graph. |
| Рестиммутаблинтрид | Неизменяемый формат идентификатора, используемый Microsoft Graph. |

Двоичные форматы (`entryId` и `immutableEntryId`) являются безопасными в URL-адресах в кодировке Base64. Безопасность URL реализована путем изменения кодировки base64 двоичных данных следующим образом:

- Замените `+` на`-`
- Замените `/` на`_`
- Удалите все замыкающие символы заполнения (`=`).
- Добавьте целое число в конец строки, указывающую количество заполненных символов в исходной (`0`, `1`или `2`).

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод `200 OK` возвращает код отклика и коллекцию [конвертидресулт](../resources/convertidresult.md) в тексте отклика.

## <a name="example"></a>Пример

В приведенном ниже примере показано, как преобразовать несколько идентификаторов из стандартного формата REST API`restId`() в неизменяемый формат REST`restImmutableEntryId`().

### <a name="request"></a>Запрос

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

### <a name="response"></a>Отклик

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
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Javascript-snippets.md)]

# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
