# <a name="delete-plannertask"></a>Удаление объекта plannerTask

Удаление объекта **plannerTask**.
### <a name="prerequisites"></a>Необходимые условия
Для выполнения этого API требуются следующие **разрешения**: 

*Group.ReadWrite.All*
### <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/<id>
```
### <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Authorization  | Bearer <code>|
| If-Match  | Последнее известное значение ETag удаляемого объекта **plannerTask**. Обязательный.|

### <a name="request-body"></a>Основной текст запросов
Не указывайте тело запроса для этого метода.


### <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает никакие данные в тексте ответа.

Этот метод может возвращать любые [коды состояния HTTP](../../../concepts/errors.md). Приложения должны обрабатывать ошибки 400, 403, 404, 409 и 412, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner_overview.md#common-planner-error-conditions).

### <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/tasks/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->