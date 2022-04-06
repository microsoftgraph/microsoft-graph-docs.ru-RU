---
author: JeremyKelley
title: Создание пакета
description: Создание пакета driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dc6f1cf54cc615b65abe3573a9b6481f83a9f3be
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561683"
---
# <a name="create-bundle"></a>Создание пакета

Пространство имен: microsoft.graph

Добавьте новый [пакет][] в диск пользователя.

[bundle]: ../resources/bundle.md

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.                             |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All   |
|Для приложений          | Не поддерживается.                                           |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание  |
|:------------- |:------------ |
| Authorization | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В корпусе запроса поставляем представление JSON созданного пакета.

## <a name="response"></a>Отклик

Если запрос будет успешным, будет возвращен [driveItem](../resources/driveitem.md) , представляющий только что созданный пакет.

Сведения об ответах на ошибки см. в этой [информации][error-response].

## <a name="examples"></a>Примеры

### <a name="example-1-create-a-bundle"></a>Пример 1. Создание пакета

В следующем примере показано, как создать базовый новый пакет.
Этот запрос создаст новый пакет с именем `Just some files` и добавит в пакет два существующих элементов.
Этот пакет можно использовать для обмена файлами с другими пользователями, не делясь папкой, в которая хранятся эти элементы.

#### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "create-bundle" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```

#### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2
  }
}
```

Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.

### <a name="example-2-create-an-album"></a>Пример 2. Создание альбома

Запрос на создание нового фотоальбома схож, хотя в аспекте пакета свойство альбомов занигается до значения non-null.

#### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "create-album" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```

#### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2,
    "album": { }
 }
}
```

Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.

Если _@microsoft.graph.conflictBehavior_ будет переименован и пакет с тем  же именем уже существует, новое имя пакета будет обновлено, чтобы быть уникальным.
OneDrive будет придать номер в конце имени пакета.

Например, будет `My Day at the Beach` переименовано `My Day at the Beach 1`.
Если `My Day at the Beach 1` будет принято, то номер будет приращен еще раз, пока не будет обнаружено уникальное имя пакета.


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Create"
} -->


