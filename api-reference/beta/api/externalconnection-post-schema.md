---
title: Создание схемы
description: Создайте схему для подключения поиска Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 98ccc34bc2e2f26223439a8f87e70ceff3b1589f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938655"
---
# <a name="create-schema"></a>Создание схемы

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте схему для [подключения](../resources/externalconnection.md)поиска Microsoft Search.

Поддерживаются два типа схем: настраиваемые элементы и файлы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Екстерналитем. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /external/connections/{id}/schema
```

## <a name="request-headers"></a>Заголовки запросов

| Имя                  | Описание                                          |
|:----------------------|:-----------------------------------------------------|
| Авторизация         | Bearer {токен}. Обязательный.                            |
| Content-Type          | application/json. Обязательный.                          |
| Предпочитать: ответ — Async | Используйте этот параметр, чтобы запрос выполнялся асинхронно. Необязательный параметр. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [схемы](../resources/schema.md) в формате JSON.

При регистрации настраиваемой схемы `schema` элемента объекту должно быть присвоено `baseType` свойство, которое `microsoft.graph.externalItem` должно содержать `properties` свойство. `properties` Объект должен содержать по крайней мере одно свойство (не более 64).

При регистрации схемы файла для `schema` `baseType` `microsoft.graph.externalFile`свойства объекта должно быть задано значение.

## <a name="response"></a>Отклик

Если `Prefer: respond-async` заголовок включен в запрос, в случае успешного выполнения этот метод возвращает код `202 Accepted` ОТКЛИКА и URL-адрес в `Location` заголовке ответа, который можно использовать для [получения состояния операции](../api/connectionoperation-get.md).

Без `Prefer: respond-async` заголовка, включенного в запрос (при успешном выполнении) Этот метод `201 Created` возвращает код отклика и новый объект [Schema](../resources/schema.md) в тексте отклика.

> [!NOTE]
> Создание схемы — длительный процесс, который может допустить превышение времени ожидания шлюза. Рекомендуется использовать `Prefer: respond-async` параметр, чтобы избежать ошибок времени ожидания.

## <a name="examples"></a>Примеры

### <a name="example-1-register-custom-schema-asynchronously"></a>Пример 1: асинхронная Регистрация настраиваемой схемы

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosohr/schema
Content-type: application/json
Prefer: respond-async

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "title",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```

### <a name="example-2-register-file-schema-synchronously"></a>Пример 2: синхронная регистрация схемы файлов

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a>Запрос
<!-- markdownlint-enable MD024 -->

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection"
}-->

```http
POST https://graph.microsoft.com/beta/connections/contosofiles/schema
Content-type: application/json

{
  "baseType": "microsoft.graph.externalFile"
}
```

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
} -->

```http
HTTP/1.1 201 Created

{
  "baseType": "microsoft.graph.externalFile"
}
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
