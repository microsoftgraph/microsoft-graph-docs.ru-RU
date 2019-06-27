---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение специальных папок
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b28f7044847bc85b9bde1d2a50ab444b64d70dcb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277100"
---
# <a name="get-a-special-folder-by-name"></a>Получение доступа к специальной папке по ее имени

Используйте специальную коллекцию для доступа к специальной папке по имени.

Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.

Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.

> **Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|            Тип разрешения             |                                           Разрешения (в порядке повышения привилегий)                                            |
| :------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All                            |
| Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite.AppFolder, Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |
| Для приложений                            | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All                                                         |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-special-folder", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}
```

### <a name="special-folder-names"></a>Имена специальных папок

Указанные ниже имена специальных папок доступны в OneDrive и OneDrive для бизнеса.

| Имя        | Идентификатор папки    | Описание                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| Документы   | `documents`  | Папка "Документы".                                                    |
| Фотографии      | `photos`     | Папка "Фотографии".                                                       |
| Альбом камеры | `cameraroll` | Папка для резервных копий альбома камеры.                                           |
| Корневая папка приложения    | `approot`    | Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}` |
| Музыка       | `music`      | Папка "Музыка".                                                        |


### <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand` и `$select` для настройки отклика.

## <a name="response"></a>Отклик

Этот метод возвращает код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.

Вы можете использовать этот метод обращения к специальной папке наряду с дополнительными вызовами к свойствам или связям в ресурсе driveItem.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "Documents",
  "eTag": "012345819293.1",
  "specialFolder": {
    "name": "documents"
  }
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-special-folder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-special-folder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-special-folder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-children-of-a-special-folder"></a>Получение дочернего элемента специальной папки

Чтобы получить дочерний элемент специальной папки, вы можете запросить коллекцию `children` или использовать параметр [expand](/graph/query-parameters) для расширения коллекции дочерних элементов.

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/special/{special-folder-name}/children
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048 },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ]
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-special-children-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-special-children-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-special-children-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a>Замечания

> **Примечание.** Элементы DriveItem с аспектом `specialFolder` указывают, что элемент представляет собой специальную папку, и доступ к нему можно получить через коллекцию `special`.

Если у вашего приложения есть разрешения только для чтения, то запрос на получение специальной папки или ее дочерних элементов может завершиться ошибкой `404 Not Found` или `403 Forbidden`, если специальная папка еще не существует.

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get-specialfolder.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
