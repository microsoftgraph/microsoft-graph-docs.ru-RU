---
title: Создание схемы
description: Создайте схему для Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b6656dc04a69c75b4803df59ee9387c4ca0fa72d
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366773"
---
# <a name="create-schema"></a>Создание схемы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте схему подключения [Поиск (Майкрософт).](../resources/externalconnection.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | ExternalItem.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a>Заголовки запросов

| Имя                  | Описание                                                        |
|:----------------------|:-------------------------------------------------------------------|
| Авторизация         | Bearer {токен}. Обязательный.                                          |
| Content-Type          | application/json. Обязательный.                                        |
| Предпочитаете: respond-async | Используйте это, чтобы вызвать асинхронное выполнение запроса. Необязательный параметр. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [схемы.](../resources/schema.md)

При регистрации настраиваемой схемы элементов объект должен иметь свойство, к котором должно быть установлено свойство, `schema` `baseType` и должен содержать `microsoft.graph.externalItem` `properties` его. Объект должен содержать по крайней мере одно свойство, не `properties` более 64.

## <a name="response"></a>Отклик

Если заготка включена в запрос, этот метод возвращает код ответа и URL-адрес в загонах ответа, которые можно использовать для получения состояния `Prefer: respond-async` `202 Accepted` `Location` [операции.](../api/connectionoperation-get.md)

Без заголовка, включенного в запрос, в случае успешного использования этот метод возвращает код ответа и новый объект схемы в `Prefer: respond-async` `201 Created` тексте ответа. [](../resources/schema.md)

> [!NOTE]
> Создание схемы — это длительный процесс, склонный к выходу времени шлюза. Рекомендуется использовать `Prefer: respond-async` заготку, чтобы избежать ошибок в периодике.

## <a name="examples"></a>Примеры

### <a name="example-register-custom-schema-asynchronously"></a>Пример. Регистрация настраиваемой схемы асинхронно

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schema-from-connection-async-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


