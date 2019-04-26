---
title: 'Страница: copyToSection'
description: Копирует страницу в определенный раздел.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 3ba56a8f5723a7f00b61e59b7ba2e40c7fbb59ce
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337911"
---
# <a name="page-copytosection"></a>Страница: copyToSection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Копирует страницу в определенный раздел.

Для операций копирования необходимо использовать шаблон асинхронного вызова: сначала вызвать действие Copy, а затем опросить конечную точку операции, чтобы получить результат.

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
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |
| Content-Type | string | `application/json` |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите объект JSON, содержащий необходимые для операции параметры.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|siteCollectionId|String|Идентификатор сайта SharePoint, в который необходимо скопировать. Используйте только при копировании на сайт группы Office 365.|
|siteId|String|Идентификатор веб-сайта SharePoint, в который необходимо скопировать. Используйте только при копировании на сайт группы Office 365.|
|groupId|String|Идентификатор группы, в которую будет копироваться. Используйте только при копировании в группу Office 365.|
|id|String|Обязательный. Идентификатор раздела назначения.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `202 Accepted` код отклика `Operation-Location` и заголовок. Опросить конечную точку Operations to Location, чтобы [получить состояние операции копирования](onenoteoperation-get.md).

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a>Отклик
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
<!--
{
  "type": "#page.annotation",
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
