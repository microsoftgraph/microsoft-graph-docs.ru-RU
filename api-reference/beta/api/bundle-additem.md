---
author: JeremyKelley
ms.author: jeremyke
title: Добавление элемента в пакет
description: Добавление элемента в пакет элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 910054e5077c8d69939a14c42db824dd862141d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987780"
---
# <a name="add-item-to-a-bundle"></a>Добавление элемента в пакет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавление дополнительного [driveItem][] с диска в [пакет][].

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.                             |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All   |
|Для приложений          | Не поддерживается.                                           |

## <a name="http-request"></a>HTTP-запрос

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание  |
|:------------- |:------------ |
| Authorization | Носитель \{токен\}. Обязательно. |

## <a name="request-body"></a>Тело запроса

Текст запроса включает идентификатор для элемента, который следует добавить в коллекцию Children набора.

## <a name="response"></a>Отклик

В случае успеха отклика `204 No Content` .

Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Этот запрос добавит существующий элемент в указанный пакет.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section": "documentation"
} -->


