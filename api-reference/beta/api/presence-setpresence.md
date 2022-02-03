---
title: 'присутствие: setPresence'
description: Установите сведения о присутствии для сеанса присутствия приложения пользователя.
author: mkhribech
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: c5060f956b4b965ca6918934bc2d1b8bdd5847a0
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341595"
---
# <a name="presence-setpresence"></a>присутствие: setPresence

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Установите состояние доступности и активности в сеансе присутствия приложения для пользователя.

### <a name="presence-sessions"></a>Сеансы присутствия
У пользователя может быть несколько сеансов присутствия, так как он может быть на нескольких Teams (настольных, мобильных и веб-). Каждый Teams клиент имеет сеанс независимого присутствия, а присутствие пользователя — это агрегированное состояние из всех сеансов позади.

Кроме того, приложение может иметь свое собственное сеанс присутствия для пользователя и иметь возможность обновлять состояние.

Ниже приводится преимущество агрегированного состояния сеанса с "A > B", представляющим приоритет над B:
* Состояние, предпочитаемого пользователем, > уровне сеанса (предпочитаемая пользователем состояние переопределяет состояния уровня сеанса)
* Среди уровней сеанса: DoNotDisturb (в настоящее время не поддерживается для **setPresence**) > Busy > Доступно > Away

### <a name="timeout-expiration-and-keep-alive"></a>Время ожидания, срок действия и сохранение
Сеанс присутствия **может быть** отсуттсвуем и **истекает,** поэтому приложению необходимо вызвать этот API перед выходом **времени, чтобы** сохранить состояние сеанса; или до **истечения срока** действия, чтобы сохранить сеанс в живых.

Сеанс присутствия может быть отсуттсвуем `Available` , если доступность и время в 5 минут. При разовом периоде состояние присутствия постепенно исчезает. Например, если `Available/Available`приложение задает сеанс присутствия в качестве, `Available/AvailableInactive` состояние изменится на 5 минут с первым таймаутом, `Away/Away` а затем через 5 минут со вторым таймаутом.

Срок действия сеанса присутствия настраивается с помощью параметра `expirationDuration` . По истечении срока действия сеанса он становится `Offline`.

## <a name="permissions"></a>Разрешения
Для вызова API требуется следующее разрешение. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Presence.ReadWrite                          |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/setPresence
```
## <a name="request-headers"></a>Заголовки запроса
| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр          | Тип     | Описание                                                                                            |
| :----------------- | :------- | :----------------------------------------------------------------------------------------------------- |
| sessionId          | string   | ID сеанса присутствия приложения.                                                          |
| availability       | string   | Сведения о базовом присутствии.                                                                         |
| действие           | string   | Дополнительные сведения о доступности.                                                          |
| expirationDuration | duration | Срок действия сеанса присутствия приложения. Значение представлено в формате ISO 8601 для длительности.</p>Если это не предусмотрено, по умолчанию будет применяться 5-минутный срок действия. |

> [!IMPORTANT]
>
> Предоставление ID приложения, как и `sessionId` в запросе.

Поддерживаемые сочетания `availability` и `activity` являются:

| availability | действие          | Описание                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| Доступно    | Доступно         | Обновляет сеанс присутствия как доступный.               |
| Занята         | InACall           | Обновляет сеанс присутствия как Busy, InACall.           |
| Занята         | InAConferenceCall | Обновляет сеанс присутствия как Busy, InAConferenceCall. |
| Away         | Away              | Обновляет сеанс присутствия как Away.                    |

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK`.

## <a name="examples"></a>Примеры
В следующем запросе показано приложение с ИД `22553876-f5ab-4529-bffb-cfe50aa89f87` , которое задает сеанс присутствия для пользователя `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "set-presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87",
  "availability": "Available",
  "activity": "Available",
  "expirationDuration": "PT1H"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/set-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/set-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/set-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/set-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/set-presence-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/set-presence-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
