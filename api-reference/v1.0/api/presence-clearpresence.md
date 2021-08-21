---
title: 'присутствие: clearPresence'
description: Очистка сведений о присутствии для сеанса присутствия приложения пользователя.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 50139466774cbecd0ef1fe87addfb7bd4d2886a2
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453837"
---
# <a name="presence-clearpresence"></a>присутствие: clearPresence

Пространство имен: microsoft.graph

Очистить сеанс присутствия приложения для пользователя. Если это единственный сеанс присутствия пользователя, его присутствие изменится на `Offline/Offline` .

Сведения о сеансах присутствия см. в материале [presence: setPresence.](presence-setpresence.md#presence-sessions)

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
При успешном выполнении этот метод возвращает код отклика `200 OK`.

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
