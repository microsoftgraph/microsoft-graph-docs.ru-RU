---
author: swapnil1993
title: Получить columnDefinition
description: Получите сайт, список или столбец типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: fee5b84275174ad6afb1bcd785f45f44e86fac12
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696744"
---
# <a name="get-columndefinition"></a>Получить columnDefinition
Пространство имен: microsoft.graph


Извлечение метаданных для [сайта,][] [списка][]или [столбца contentType.][] [][columnDefinition]

  

## <a name="permissions"></a>Разрешения

  

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All  |

  

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /sites/{site-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}/columns/{column-id}
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|  

## <a name="request-body"></a>Тело запроса

  

Не указывайте текст запроса для этого метода.

  

## <a name="example"></a>Пример

  

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "get_column_from_contenttype" } -->

  

```http
GET /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```

### <a name="response"></a>Отклик

  

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "readOnly": false,
  "required": false,
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md

[list]: ../resources/list.md

[site]: ../resources/site.md

[contentType]: ../resources/contentType.md
  
