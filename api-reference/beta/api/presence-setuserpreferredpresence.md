---
title: 'присутствие: setUserPreferredPresence'
description: Настройка предпочитаемого пользователем присутствия для пользователя
author: mkhribech
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 005c0c6cd0f35455780c11650a10bab96280bc6d
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526097"
---
# <a name="presence-setuserpreferredpresence"></a>присутствие: setUserPreferredPresence

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Установите предпочтительное состояние доступности и активности для пользователя. Если установлено предпочтительное присутствие пользователя, его присутствие является предпочтительным.

Предпочтительное присутствие вступает в силу только при наличии хотя бы [одного](presence-setpresence.md#presence-sessions) сеанса присутствия пользователя. В противном случае присутствие пользователя остается в автономном режиме.

Сеанс присутствия может быть создан в результате успешной операции [setPresence](presence-setpresence.md) или если пользователь подписан на Teams клиента. 

Дополнительные новости о [сеансах присутствия](presence-setpresence.md#presence-sessions) и [их времени ожидания и истечения срока действия.](presence-setpresence.md#timeout-expiration-and-keep-alive) 

## <a name="permissions"></a>Permissions
Для вызова API требуется следующее разрешение. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Presence.ReadWrite                          |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/setUserPreferredPresence
```
## <a name="request-headers"></a>Заголовки запроса
| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр          | Тип     | Описание                                                                                                                                                                                                                                    |
| :----------------- | :------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| availability       | строка   | Сведения о базовом присутствии.                                                                                                                                                                                                                 |
| действие           | string   | Дополнительные сведения о доступности.                                                                                                                                                                                                  |
| expirationDuration | duration | Срок действия сеанса присутствия приложения. Значение представлено в формате ISO 8601 для длительности.<br/>В случае невыполнения условий по умолчанию будет применено:<br/>DoNotDisturb или Busy: срок действия истекает через 1 день<br/>Все остальные: срок действия истекает через 7 дней |

Поддерживаемые сочетания **доступности** и **активности:**

| availability | действие     | Описание                                         |
| :----------- | :----------- | :-------------------------------------------------- |
| Доступно    | Доступно    | Установите предпочтительное присутствие пользователя как доступное.       |
| Занята         | Занята         | Установите предпочтительное для пользователя присутствие как Busy.            |
| DoNotDisturb | DoNotDisturb | Установите предпочтительное присутствие пользователя как DoNotDisturb.    |
| BeRightBack  | BeRightBack  | Установите предпочтительное присутствие пользователя как BeRightBack.     |
| Away         | Away         | Установите предпочтительное для пользователя присутствие как Away.            |
| Автономный режим      | OffWork      | Установите предпочтительное для пользователя присутствие в автономном режиме. |

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK`.

## <a name="examples"></a>Примеры

Следующий запрос задает пользователю предпочтительное присутствие в качестве DoNotDisturb для пользователя `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` с истечением 8 часов.

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "setUserPreferredPresence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setUserPreferredPresence
Content-Type: application/json

{
  "availability": "DoNotDisturb",
  "activity": "DoNotDisturb",
  "expirationDuration": "PT8H"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/setuserpreferredpresence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/setuserpreferredpresence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/setuserpreferredpresence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/setuserpreferredpresence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/setuserpreferredpresence-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
