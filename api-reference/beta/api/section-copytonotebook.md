---
title: 'section: copyToNotebook'
description: Копирование раздела в указанную записную книжку.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 65a3dd079f0ed67e7c754f22f805de8ed8368c87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928208"
---
# <a name="section-copytonotebook"></a>section: copyToNotebook

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Копирование раздела в указанную записную книжку.

Для операций Copy необходимо использовать модель асинхронного вызова:  сначала вызовите действие Copy, а затем опросите конечную точку операции, чтобы получить результат.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Notes.Create, Notes.ReadWrite    |
|Для приложений | Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |
| Content-Type | строка | `application/json` |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите объект JSON, который содержит параметры, требуемые операцией.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|siteCollectionId|String|Идентификатор сайта SharePoint для копирования. Используйте только при копировании на сайте группы разработчиков Office 365.|
|siteId|String|Идентификатор веб-сайта SharePoint, чтобы скопировать. Используйте только при копировании на сайте группы разработчиков Office 365.|
|groupId|String|Идентификатор группы, в которую необходимо выполнить копирование. Используется только при копировании в группу Office 365.|
|id|Строка|Обязательный. Идентификатор целевой записной книжки. |
|renameAs|String|Имя копии. По умолчанию используется имя существующего элемента. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа `202 Accepted` и заголовок `Operation-Location`. [Чтобы получить сведения о состоянии операции копирования](onenoteoperation-get.md), опросите конечную точку Operation-Location.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a>Ответ
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
