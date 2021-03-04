---
author: swapnil1993
ms.date: 08/30/2020
title: Создание columnDefinition
description: Добавление столбца в тип контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 071a855c79c055179022157b991b4a9f2789cad1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447230"
---
# <a name="create-columndefinition"></a>Создание columnDefinition
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Добавляет существующий столбец [столбец]сайта или[спискаDefinition] в [контент типа][контентаType.]

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/concepts/permissions_reference.md).

  

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/contentTypes/{contentType-id}/columns
POST /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns
```

## <a name="request-body"></a>Тело запроса

В теле запроса добавьте представление JSON ресурса [columnDefinition.][]  

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект contentType][] в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
    "sourceColumn@odata.bind": "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
}
```

### <a name="response"></a>Отклик

Ответ возвращает список всех столбцов, добавленных в тип контента.

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true, "scopes": "sites.readwrite.all" } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}

```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
  

