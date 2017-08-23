# <a name="move-a-driveitem"></a>Перемещение ресурса DriveItem

Чтобы переместить ресурс DriveItem в новый родительский элемент, веб-приложению требуется обновить элемент **parentReference** из DriveItem. Это особый случай, касающийся метода [Обновление](item_update.md). Приложение может объединять процедуры перемещения элемента в новый контейнер и обновления других свойств элемента в один запрос.

С помощью этого запроса невозможно перемещать элементы между объектами [Drive](../resources/drive.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | 
|:--------------------|:---------------------------------------------------------| 
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    | 
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    | 
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All | 

## <a name="http-request"></a>HTTP-запрос

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-match      | String | Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`. |


## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте новое значение для поля свойства **parentReference**. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в другие значения свойств. Чтобы производительность была максимальной, не следует включать существующие значения, которые не изменились.

**Примечание.** При перемещении элементов в корень OneDrive не следует использовать синтаксис `"id:" "root"`. Нужно использовать действительный идентификатор корневой папки или путь `{"path": "/drive/root"}` для родительской ссылки.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.

## <a name="example"></a>Пример
В этом примере элемент, определяемый идентификатором элемента {item-id}, перемещается в папку **Документы** в OneDrive пользователя.

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

##### <a name="response"></a>Отклик

Ниже приводится пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
