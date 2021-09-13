---
title: Обновление объекта conversationThread
description: Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e4777a0dc2942451b23733a0a8bc7b7a37e46000
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063526"
---
# <a name="update-conversationthread"></a>Обновление объекта conversationThread

Пространство имен: microsoft.graph

Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{group id}/threads/{thread id}
PATCH /groups/{group id}/conversations/{conversation id}/threads/{thread id}

```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|isLocked|Логическое|Указывает, заблокирована ли цепочка. Чтобы запретить добавление сообщений, задайте значение `true`.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` пустой объект в тексте отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "ignored",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/0fbf2921-5d17-4c2b-bae4-cc581de72c13/threads/AAQkAGU3OGZjZTE2LTFlOWItNGExYi1hMGMzLTMwZWU4OGUzYjU5MQMkABAALmW2hn6Ui0_7hOBeAIFdWhAALmW2hn6Ui0_7hOBeAIFdWg==
Content-type: application/json

{
  "isLocked": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

