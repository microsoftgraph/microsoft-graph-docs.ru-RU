# <a name="delete-contact"></a>Удаление контакта

Удаление контакта.
## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется одна из указанных **областей**: *Contacts.ReadWrite*
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer <token>. Обязательный параметр.  |

## <a name="request-body"></a>Тело запроса
Не указывайте тело запроса для этого метода.


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
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
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
