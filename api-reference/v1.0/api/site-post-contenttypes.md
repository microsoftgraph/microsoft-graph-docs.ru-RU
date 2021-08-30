---
author: swapnil1993
title: Создание типа контента
description: Создание типа контента на сайте.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 07517bca0d176bcc2f63e93f26159f079c4ede8b
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696840"
---
# <a name="create-a-content-type"></a>Создание типа контента
Пространство имен: microsoft.graph

Создание нового [contentType][] на [сайте.][]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |Sites.Manage.All, Sites.FullControl.All    |
|Делегированные (личная учетная запись Майкрософт) |Не поддерживается    |
|Приложение |Sites.Manage.All, Sites.FullControl.All |


## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/contentTypes
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON для создания [ресурса contentType.][]

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект contentType][] в тексте ответа.


## <a name="example"></a>Пример

В следующем примере показано, как создать новый тип общего контента.

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_contenttype"
}
-->

```http
POST https://graph.microsoft.com/v1.0/sites/{id}/contentTypes
Content-Type: application/json

{
    "name": "docSet",
    "description": "custom docset",
    "base": {
        "name": "Document Set",
        "id": "0x0120D520"
    },
    "group": "Document Set Content Types" 
}
```

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "0x01002A2479FF33DD4BC3B1533A012B653717",
  "name": "docSet",
  "group":"Document Set Content Types",
  "description" : "custom docset",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```


[contentType]: ../resources/contentType.md
[site]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a content type in a site",
  "keywords": "content type",
  "section": "documentation",
  "tocPath": "sites/Create ContentType",
  "suppressions": [
  ]
}
-->
