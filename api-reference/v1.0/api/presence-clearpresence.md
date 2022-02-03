---
title: 'присутствие: clearPresence'
description: Очистка сведений о присутствии для сеанса присутствия приложения пользователя.
author: jsandoval-msft
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: aeb16ea81e475cbc100099b1a61732cc485d886d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348628"
---
# <a name="presence-clearpresence"></a>присутствие: clearPresence

Пространство имен: microsoft.graph

Очистить сеанс присутствия приложения для пользователя. Если это единственный сеанс присутствия пользователя, его присутствие изменится на `Offline/Offline`.

Сведения о сеансах присутствия см. в материале [presence: setPresence](presence-setpresence.md#presence-sessions).

## <a name="permissions"></a>Разрешения
Для вызова API требуется следующее разрешение. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.                              |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearPresence
```

## <a name="request-headers"></a>Заголовки запроса
| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {token}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр | Тип   | Описание                                   |
| :-------- | :----- | :-------------------------------------------- |
| sessionId | string | ID сеанса присутствия приложения. |


> [!IMPORTANT]
> 
> Предоставление ID приложения, как и `sessionId` в запросе.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK`.

Если сеанс присутствия не существует, этот метод возвращает код `404 NotFound` ответа.

## <a name="examples"></a>Примеры
В следующем запросе показано приложение с ИД `22553876-f5ab-4529-bffb-cfe50aa89f87` , которое очищает сеанс присутствия для пользователя `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clear--presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clear--presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clear--presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clear--presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clear--presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/clear--presence-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/clear--presence-powershell-snippets.md)]
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
