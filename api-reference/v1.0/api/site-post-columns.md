---
author: swapnil1993
ms.date: 08/30/2020
title: Создание столбцаDefinition на сайте
description: Создание столбца сайта.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5953cde6c75f3b807d87fd8f77b8f563ad43819c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696845"
---
# <a name="create-a-columndefinition-in-a-site"></a>Создание столбцаDefinition на сайте
Пространство имен: microsoft.graph

Создание столбца для [сайта][site] with a request that specifies a [columnDefinition][columnDefinition] .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/concepts/permissions_reference.md).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Manage.All, Sites.FullControl.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение | Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/columns
```

## <a name="request-body"></a>Текст запроса

В теле запроса добавьте представление JSON ресурса [columnDefinition.][]  

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект columnDefinition][] в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
<!-- { "blockType": "request", "name": "site_post_columns" } -->
```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/columns
Content-Type: application/json

{
   "description":"test",
   "enforceUniqueValues":false,
   "hidden":false,
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "description":"test",
   "displayName":"Title",
   "enforceUniqueValues":false,
   "hidden":false,
   "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[site]: ../resources/site.md
  

