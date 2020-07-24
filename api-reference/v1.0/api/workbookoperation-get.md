---
title: Получение Воркбукоператион
description: Получение состояния объекта Воркбукоператион.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0d790d7bfc243cb5cfbc32a12d6a00db32c46cd9
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408169"
---
# <a name="get-workbookoperation"></a>Получение Воркбукоператион

Получение состояния объекта [воркбукоператион](../resources/workbookoperation.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Files. ReadWrite. |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET workbook/operations/{operation-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркбукоператион](../resources/workbookoperation.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_workbookoperation"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
```

### <a name="response"></a>Отклик

Ниже приведен ответ со статусом "работает".


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "running"
}
```

Ниже приведен ответ со статусом "выполнено успешно".

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "succeeded",
  "resourceLocation":"https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')"
}
```

Ниже приведен ответ со статусом "Failed".

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "operation-id",
  "status": "failed",
  "error":
  {
      "code": "internalServerError",
      "message": "An internal server error occurred while processing the request.",
      "innerError": {
          "code": ""internalServerErrorUncategorized",
          "message": "An unspecified error has occurred.",
          "innerError": {
               "code": "GenericFileOpenError",
               "message": "The workbook cannot be opened."
          }
      }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
