# <a name="remove-member"></a>Удаление элемента

С помощью этого API можно удалить участника из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации **members**. Вы можете удалять пользователей или другие группы.

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*, *Directory.ReadWrite.All* или *Directory.AccessAsUser.All*

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | строка  | Bearer <token>. Обязательный параметр. |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->