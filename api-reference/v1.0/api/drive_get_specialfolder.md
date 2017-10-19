---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Получение специальных папок"
ms.openlocfilehash: 894c0dc2c41441ab8006f58dcf5ccbc9d0043b0a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="get-a-special-folder-by-name"></a>Получение специальной папки по ее имени

Используйте специальную коллекцию для доступа к специальной папке по имени.

Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.

Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.

> **Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

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

Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) `$expand` и `$select` для настройки ответа.

## <a name="http-response"></a>HTTP-ответ

Этот метод возвращает код ответа `200 OK` и объект [driveItem](../resources/driveitem.md) в теле ответа.

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

## <a name="get-children-of-a-special-folder"></a>Получение дочернего элемента специальной папки

Чтобы получить список дочерних элементов специальной папки, вы можете запросить коллекцию `children` либо с помощью параметра [expand](../../../concepts/query_parameters.md) расширить коллекцию дочерних элементов.

### <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-special-children", "scopes": "files.read" } -->

```http
GET /me/drive/special/{name}/children
```

### <a name="http-response"></a>HTTP-ответ

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

## <a name="remarks"></a>Примечания

> **Примечание.** Элементы DriveItem с аспектом `specialFolder` указывают, что элемент представляет собой специальную папку, и доступ к нему можно получить через коллекцию `special`.

Если у вашего приложения есть разрешения только для чтения, то запрос на получение специальной папки или ее дочерних элементов может завершиться ошибкой `404 Not Found` или `403 Forbidden`, если специальная папка еще не существует.

<!-- {
  "type": "#page.annotation",
  "description": "Access known folders in OneDrive through the special folder collection",
  "keywords": "known folders",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Special folders"
} -->
