---
title: 'presence: setPresence'
description: Задайте сведения о присутствии для сеанса присутствия приложения пользователя.
author: jsandoval-msft
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: c65754ffa61f62577ce4023d9a4a6e48ce0d533e
ms.sourcegitcommit: a11c874a7806fb5825752c8348e12079d23323e4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2022
ms.locfileid: "65293958"
---
# <a name="presence-setpresence"></a>presence: setPresence

Пространство имен: microsoft.graph

Задайте состояние сеанса присутствия пользователя в качестве приложения.

### <a name="presence-sessions"></a>Сеансы присутствия
Пользователь может иметь несколько сеансов присутствия, так как он может быть на нескольких клиентах Teams (настольных компьютерах, мобильных устройствах и Интернете). Каждый Teams имеет независимый сеанс присутствия, а присутствие пользователя — это агрегированное состояние из всех сеансов.

Аналогичным образом приложение может иметь собственный сеанс присутствия для пользователя и иметь возможность обновлять состояние.

Ниже приведен приоритет агрегирования состояний сеансов.
* Настраиваемые пользователем > приложения (пользовательское состояние переопределяет другие)
* Среди настроенных приложений: DoNotDisturb (в настоящее время не поддерживается для набора сведений о присутствии) > Занят > Доступно > Нет

### <a name="timeout-expiration-and-keep-alive"></a>Время ожидания, истечение срока действия и сохранение активности
Время ожидания сеанса  присутствия может истечь **, поэтому** приложению необходимо вызвать этот API до истечения времени **ожидания, чтобы** сохранить состояние сеанса; или до **истечения срока действия**, чтобы поддерживать сеанс в активном состоянии.

Время ожидания сеанса присутствия может истекло, `Available` если доступность и время ожидания — 5 минут. Когда время ожидания истекает, состояние присутствия постепенно исчезает. Например, если `Available/Available`приложение задает сеанс присутствия в качестве, `Available/AvailableInactive` состояние изменится на 5 минут с первым временем ожидания, `Away/Away` а затем через 5 минут со вторым временем ожидания.

Срок действия сеанса присутствия можно настроить с помощью параметра `expirationDuration` . По истечении срока действия сеанса он становится .`Offline`

## <a name="permissions"></a>Разрешения
Для вызова API требуется следующее разрешение. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Presence.ReadWrite                              |
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
| Sessionid          | строка   | Идентификатор сеанса присутствия приложения.                                                          |
| availability       | строка   | Базовые сведения о присутствии.                                                                         |
| действие           | строка   | Дополнительные сведения о доступности.                                                          |
| expirationDuration | duration | Срок действия сеанса присутствия приложения. Значение представлено в формате ISO 8601 для длительности.</p>Если этот параметр не указан, применяется срок действия по умолчанию 5 минут. Допустимый диапазон длительности — 5–240 минут (от PT5M до PT4H)|

> [!IMPORTANT]
>
> Укажите идентификатор приложения, как в `sessionId` запросе.

Поддерживаемые сочетания и`availability`:`activity`

| availability | действие          | Описание                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| Доступно    | Доступно         | Обновляет сеанс присутствия как доступный.               |
| Занята         | InACall           | Обновляет сеанс присутствия как "Занят", "InACall".           |
| Занята         | InAConferenceCall | Обновляет сеанс присутствия как "Занят", InAConferenceCall. |
| Нет на месте         | Нет на месте              | Обновляет сеанс присутствия как "Нет на месте".                    |

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK`.

## <a name="examples"></a>Примеры
В следующем запросе показано приложение с идентификатором `22553876-f5ab-4529-bffb-cfe50aa89f87` , который задает сеанс присутствия для пользователя `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.

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
