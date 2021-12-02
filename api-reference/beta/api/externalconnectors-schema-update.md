---
title: Обновление схемы
description: Обновление свойств схемы для externalConnection.
ms.localizationpriority: medium
author: mecampos
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: bd0aa8d8d37c9cf7652853b530f91627f2286974
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266443"
---
# <a name="update-schema"></a>Обновление схемы

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств [схемы](../resources/externalconnectors-schema.md) для [externalConnection](../resources/externalconnectors-externalconnection.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | ExternalConnection.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connectionId}/schema
```

## <a name="request-headers"></a>Заголовки запросов

| Имя                  | Описание                                                        |
|:----------------------|:-------------------------------------------------------------------|
| Авторизация         | Bearer {токен}. Обязательный.                                          |
| Content-Type          | application/json. Обязательный.                                        |
| Предпочитаете: respond-async | Используйте это, чтобы вызвать асинхронное выполнение запроса. Необязательно. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [схемы.](../resources/externalconnectors-schema.md)

При регистрации настраиваемой схемы элемента  объект **схемы** должен иметь свойство **baseType** и должно содержать `microsoft.graph.externalItem` свойство **свойств.**  Объект **свойств должен** **содержать** по крайней мере одно свойство, не более 128.

## <a name="response"></a>Отклик

В случае успешного использования этот метод возвращает код ответа и URL-адрес в загонах ответа, которые можно использовать для `202 Accepted` `Location` получения состояния [операции.](../api/externalconnectors-connectionoperation-get.md)

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_schema"
}-->

```http
PATCH https://graph.microsoft.com/beta/external/connections/contosohr/schema
Content-type: application/json

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "string",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "string",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "string",
      "isRetrievable": "true"
    }
  ]
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
