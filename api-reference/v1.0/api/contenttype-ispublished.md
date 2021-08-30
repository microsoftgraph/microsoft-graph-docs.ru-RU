---
author: swapnil1993
title: 'contentType: isPublished'
description: Проверьте состояние публикации типа контента на веб-узбе типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 1b50b178c49af99a630aa6a09d64222d98a0285a
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696803"
---
# <a name="contenttype-ispublished"></a>contentType: isPublished
Пространство имен: microsoft.graph


Проверьте состояние публикации [контентаType][] на веб-сайте концентратора типа контента.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.FullControl.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается   |
|Приложение | Sites.FullControl.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
>**Примечание:** _SiteId представляет_ веб-узел типа контента.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="response"></a>Отклик
В случае успешной работы этот вызов возвращает ответ и значение Boolean, которое указывает состояние публикации `200 OK` типа контента.

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```http
GET https://graph.microsoft.com/v1.0/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true 
}
```

[contentType]: ../resources/contentType.md
