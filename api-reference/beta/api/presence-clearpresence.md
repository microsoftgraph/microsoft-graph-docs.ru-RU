---
title: 'присутствие: clearPresence'
description: Очистка сведений о присутствии для сеанса присутствия приложения пользователя.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 02140f99accf36bfac156996e83bd75de2bb3b19
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107911"
---
# <a name="presence-clearpresence"></a>присутствие: clearPresence

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Очистить сеанс присутствия приложения для пользователя. Если это единственный сеанс присутствия пользователя, его присутствие изменится на `Offline/Offline` .

Сведения о сеансах присутствия см. в материале [presence: setPresence.](presence-setpresence.md#presence-sessions)

## <a name="permissions"></a>Разрешения
Для вызова API требуется следующее разрешение. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированное (рабочая или учебная учетная запись)     | Не поддерживается.                              |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearPresence
```

## <a name="request-headers"></a>Заголовки запроса
| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр | Тип   | Описание                                   |
| :-------- | :----- | :-------------------------------------------- |
| sessionId | string | ID сеанса присутствия приложения. |


> [!IMPORTANT]
> 
> Предоставление ID приложения, как `sessionId` и в запросе.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK`.

Если сеанс присутствия не существует, этот метод возвращает код `404 NotFound` ответа.

## <a name="examples"></a>Примеры
В следующем запросе показано приложение с ИД, которое очищает `22553876-f5ab-4529-bffb-cfe50aa89f87` сеанс присутствия для `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` пользователя.

### <a name="request"></a>Запрос

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

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
