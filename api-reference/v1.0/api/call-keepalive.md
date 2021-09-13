---
title: 'call: keepAlive'
description: Сделайте запрос на этот API каждые 15-45 минут, чтобы убедиться, что текущий вызов остается в живых.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a26b0b6cf2f9a3da8c19175bfbfffffd3276247b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053765"
---
# <a name="call-keepalive"></a>call: keepAlive

Пространство имен: microsoft.graph

Сделайте запрос на этот API каждые 15-45 минут, чтобы убедиться, что текущий вызов остается активным. Вызов, который не получает этот запрос в течение 45 минут, считается неактивным и впоследствии завершится.

По крайней мере один успешный запрос должен быть выполнен в течение 45 минут после предыдущего запроса или начала вызова.

Рекомендуется отправлять запрос с более короткими интервалами времени (каждые 15 минут). Убедитесь, что эти запросы являются успешными, чтобы предотвратить время и завершение вызова.

Попытка отправить запрос на уже закончившийся вызов приведет к `404 Not-Found` ошибке. Ресурсы, связанные с вызовом, должны быть очищены на стороне приложения.

## <a name="permissions"></a>Разрешения
Для вызова этого API может потребоваться одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается        |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается        |
| Для приложений     | Нет                                        |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
Этот метод возвращает код `200 OK` ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже показан пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/keep-alive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/keep-alive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/keep-alive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/keep-alive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приводится пример отклика.

<!-- {
  "blockType": "response",
  "name": "keep-alive",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```


<!--
{
  "type": "#page.annotation",
  "description": "call: keepAlive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

