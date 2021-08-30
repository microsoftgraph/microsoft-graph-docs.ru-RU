---
author: swapnil1993
title: 'contentType: неопубликованный'
description: Отопубликуй тип контента с сайта концентратора типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: f93c86721fb3f1fd030188b5a0b20e3946fdb86c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696816"
---
# <a name="contenttype-unpublish"></a>contentType: неопубликованный
Пространство имен: microsoft.graph


Unpublish a [contentType][] from a content type hub site.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.FullControl.All    |
|Делегированные (личная учетная запись Майкрософт) | Sites.FullControl.All    |
|Приложение | Sites.FullControl.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

>**Примечание:** _SiteId представляет_ веб-узел типа контента.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает `204 No Content` ответ.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "contenttype_unpublish"
}
-->
```http
POST https://graph.microsoft.com/v1.0/sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
