---
author: JeremyKelley
title: Пакеты списков
description: Список пакетов в диске пользователя
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b4810ba395d9f04eee4b5f9a226a6abb9fc83715
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561678"
---
# <a name="list-bundles"></a>Пакеты списков

Пространство имен: microsoft.graph

Получите список всех [пакетов] [в] диске пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.                             |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Для приложений          | Не поддерживается.                                           |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData][] для фильтрации и формирования ответа.

Параметр запроса нельзя использовать `expand=children` при переумеживании пакетов.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание  |
|:------------- |:------------ |
| Authorization | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот запрос возвращает список элементов пакета, определенных для диска.

Сведения об ответах на ошибки см. в этой [информации][error-response].

## <a name="examples"></a>Примеры

### <a name="example-1-list-all-bundles-in-a-drive"></a>Пример 1. Список всех пакетов в диске

Чтобы запросить переопределение всех пакетов, определенных в диске, можно сделать запрос в коллекцию пакетов без параметров.

#### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles
```

#### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "0120310201abd",
      "name": "Family shared files",
      "bundle": {
        "childCount": 1
      }
    }
  ],
  "@odata.nextLink": "https://..."
}
```

Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.


### <a name="example-2-list-all-photo-albums-in-a-drive"></a>Пример 2. Список всех фотоальбомов на диске

Чтобы отфильтровать список пакетов, возвращаемого из запроса в коллекцию пакетов, `filter` можно использовать параметр строки запроса, чтобы указать тип пакета, чтобы вернуться, проверив наличие грани в пакете:

#### <a name="request"></a>Запрос

<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```

#### <a name="response"></a>Отклик

Ответ на GET для конечной точки пакетов — массив ресурсов [driveItem][] с [пакетом][].
Так как все пакеты являются элементами, можно использовать все стандартные операции элемента на них.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true, "isCollection": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0123456789abc",
      "name": "Vacation photo album",
      "bundle": {
        "childCount": 1,
        "album": { }
      }
    },
    {
      "id": "120301010abcd",
      "name": "Seattle Center event",
      "bundle": {
        "childCount": 4,
        "album": { }
      },
      "tags": [
        {
          "name": "outside",
          "autoTagged": { }
        }
      ]
    }
  ]
}
```

Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors
[Параметры запроса OData]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "List the bundles in a drive.",
  "keywords": "list,bundle,collection",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/List"
} -->


