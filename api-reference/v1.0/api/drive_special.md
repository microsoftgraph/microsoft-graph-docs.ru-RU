# <a name="get-a-special-folder-by-name"></a>Получение доступа к специальной папке по имени

Используйте специальную коллекцию для доступа к специальной папке по имени.

Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.

Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.

**Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**:

* Files.Read
* Files.ReadWrite.
* Files.Read.All
* Files.ReadWrite.All
* Files.ReadWrite.AppFolder
* Sites.Read.All
* Sites.ReadWrite.All

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание               |
|:--------------|:-------|:--------------------------|
| Authorization | string | Bearer {токен}. Обязательный. |


## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос
Ниже приведен пример запроса на получение списка дисков пользователя.

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a>Заметки

Чтобы получить список дочерних элементов для специальной папки, можно запросить коллекцию `children` или с помощью параметра [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) развернуть этот список.


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
