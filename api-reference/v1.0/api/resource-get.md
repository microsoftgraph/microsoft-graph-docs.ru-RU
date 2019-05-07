---
title: Вывод ресурса
description: Получение двоичных данных объекта ресурса файла или изображения.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 1b94486936d6e0ffc916bdcd4acfe895ad5e97f7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603759"
---
# <a name="get-resource"></a>Вывод ресурса

Получение двоичных данных объекта [ресурса](../resources/resource.md) файла или изображения.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Notes. Read, Notes. ReadWrite    |
|Для приложений | Notes.Read.All, Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и двоичные данные изображения или файла в тексте отклика.

Note: изображения не отображаются непосредственно в браузере, так как им требуется авторизация для их извлечения, как и остальная часть контента страницы.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```
#### <a name="sdk-sample-code"></a>Пример кода для SDK
# <a name="ctabcs"></a>[Языках](#tab/cs)
[!INCLUDE [sample-code](../includes/get_resource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Язык](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_resource-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/resource-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/resource-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
