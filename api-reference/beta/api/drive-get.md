---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
ms.openlocfilehash: 903eb9d5886bf2ec3b7f8672438f01482e754f9b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748593"
---
# <a name="get-drive"></a>Получение ресурса Drive

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).

Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотеки документов SharePoint.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Для приложений | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="get-current-users-onedrive"></a>Получение хранилища OneDrive текущего пользователя

Доступ к объекту drive пользователя, вошедшего в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.

Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен объект drive пользователя (при использовании делегированной проверки подлинности).

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a>Получение хранилища OneDrive пользователя

Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.

Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен объект drive пользователя (при использовании делегированной проверки подлинности).

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a>Параметры пути

| Имя параметра | Значение  | Описание                                       |
|:---------------|:-------|:--------------------------------------------------|
| _idOrUserPrincipalName_     | строка | Обязательный. Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive. |

## <a name="get-the-document-library-associated-with-a-group"></a>Получение библиотеки документов, сопоставленной с группой

Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a>Параметры пути

| Имя параметра | Значение  | Описание                                       |
|:---------------|:-------|:--------------------------------------------------|
| _groupId_      | строка | Обязательный. Идентификатор группы, которой принадлежит библиотека документов. |

## <a name="get-the-document-library-for-a-site"></a>Получение библиотеки документов для сайта

Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.

### <a name="http-request"></a>HTTP-запрос

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a>Параметры пути

| Имя параметра | Значение  | Описание                                       |
|:---------------|:-------|:--------------------------------------------------|
| _siteId_       | строка | Обязательный. Идентификатор для сайта, который содержит библиотеку документов. |

## <a name="get-a-drive-by-id"></a>Получение объекта drive с использованием его идентификатора

Если у вас есть уникальный идентификатор drive, вы можете получить доступ к этому объекту непосредственно из коллекции объектов drive верхнего уровня.

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a>Параметры пути

| Имя параметра | Значение  | Описание                                       |
|:---------------|:-------|:--------------------------------------------------|
| _driveId_      | строка | Обязательный. Идентификатор запрошенного диска. |

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования отклика.

## <a name="response"></a>Ответ

Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего объекта drive в теле отклика.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a>Коды откликов с ошибками

Если объект drive не существует и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен отклик `HTTP 404`.

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
