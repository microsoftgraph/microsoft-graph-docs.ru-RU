---
title: Создание подключения
description: Используйте этот API для создания нового Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6b85c5a9a09690f91f3e0934512f3cc874e54b46
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938683"
---
# <a name="create-connection"></a>Создание подключения

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [екстерналконнектион](../resources/externalconnection.md).

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
POST /external/connections
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
|:--------------|:----------------------------|
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [екстерналконнектион](../resources/externalconnection.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [екстерналконнектион](../resources/externalconnection.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_connection_from_external"
}-->

```http
POST https://graph.microsoft.com/beta/external/connections
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик
<!-- markdownlint-enable MD024 -->

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "configuration": {
    "authorizedApps": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
