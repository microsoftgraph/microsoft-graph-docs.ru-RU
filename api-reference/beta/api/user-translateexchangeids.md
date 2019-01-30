---
title: 'пользователь: translateExchangeIds'
description: Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a00368c918685f6f94020dbea655232bae58ad57
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643617"
---
# <a name="user-translateexchangeids"></a>пользователь: translateExchangeIds

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Перевод идентификаторов ресурсов, связанных с Outlook, между форматами.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:----------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись) | User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | User.ReadBasic, User.Read, User.ReadWrite |
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
| inputIds | Edm.String коллекции | Коллекция идентификаторов для преобразования. Все идентификаторы в коллекции должны иметь одного идентификатор типа и значения для элементов в тот же почтовый ящик. Максимальный размер семейства сайтов составляет 1 000 строк. |
| sourceIdType | exchangeIdFormat | Тип идентификатора идентификаторов в `InputIds` параметр. |
| targetIdType | exchangeIdFormat | Запрошенный тип идентификатора для преобразования. |

### <a name="exchangeidformat-values"></a>exchangeIdFormat значения

| Значения | Описание |
|:-------|:------------|
| Идентификатор записи | Формат идентификатора двоичные запись, используемого клиентами MAPI. |
| ewsId | Идентификатор формата, используемого клиентами веб-служб Exchange. |
| immutableEntryId | Двоичные MAPI-совместимое постоянные идентификатор формата. |
| restId | По умолчанию идентификатор формата Microsoft Graph. |
| restImmutableEntryId | Постоянные идентификатор формата, используемого в Microsoft Graph. |

Двоичные форматы (`entryId` и `immutableEntryId`) являются кодировке base64 safe URL-адрес. URL-адрес safeness осуществляется путем изменения Кодировка base64 двоичных данных следующим образом:

- Замените `+` с`-`
- Замените `/` с`_`
- Удалите все конечные знаки внутренние поля (`=`)
- Добавление целое число в конец строки, показывающее, сколько символов заполнения были в исходной (`0`, `1`, или `2`)

## <a name="response"></a>Отклик

Успешно завершена, этот метод возвращает `200 OK` код ответа и семейства [convertIdResult](../resources/convertidresult.md) в теле ответа.

## <a name="example"></a>Пример

Следующем примере показано, как преобразовать несколько идентификаторов из обычного формата API-Интерфейс REST (`restId`) в формат постоянные REST (`restImmutableEntryId`).

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
