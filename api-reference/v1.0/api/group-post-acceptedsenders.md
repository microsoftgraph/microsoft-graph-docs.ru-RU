---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: dkershaw10
ms.openlocfilehash: 7a0fc795507a1c2b6a8b20407b9f72347503e507
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27300856"
---
# <a name="create-acceptedsender"></a>Создание объекта acceptedSender
Добавление пользователя или группы в список объектов acceptedSender.

Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Укажите в тексте запроса идентификатор объекта user или group.

## <a name="response"></a>Отклик
Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.

## <a name="example"></a>Пример
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```

#### <a name="response"></a>Ответ
Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
