# <a name="create-a-sharing-link-for-a-driveitem"></a>Создание ссылки для совместного доступа для ресурса DriveItem

Используя действие **createLink**, вы можете поделиться ресурсом [DriveItem](../resources/driveitem.md) с помощью ссылки для совместного доступа.

Действие **createLink** создает ссылку для совместного доступа, если ссылка указанного типа еще не существует для приложения, совершающего вызов. Если для приложения уже создана такая ссылка указанного типа, возвращается она.

Ресурсы DriveItem наследуют разрешения от своих предков.

## <a name="prerequisites"></a>Необходимые компоненты
Для применения этого API требуется одна из указанных **областей**:

  * Files.ReadWrite

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a>Текст запроса
В теле запроса определяется тип ссылки для совместного доступа, нужной приложению. Запрос должен содержать объект JSON с указанным ниже свойством.

| Имя      | Тип   | Описание                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| **type**  | string | Тип создаваемой ссылки для совместного доступа. Возможные значения: `view`, `edit` или `embed`.       |
| **scope** | string | Область создаваемой ссылки. Возможные значения: `anonymous` или `organization`. Необязательный параметр. |

## <a name="link-types"></a>Типы ссылок
Параметр **type** может принимать указанные ниже значения.

| Значение типа | Описание                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | Создает ссылку на элемент, предполагающую доступ только для чтения.                                                        |
| `edit`     | Создает ссылку на элемент, предполагающую доступ для чтения и записи.                                                       |
| `embed`    | Создает встроенную ссылку на элемент. Этот вариант доступен только для личных учетных записей OneDrive. |

## <a name="scope-types"></a>Типы областей
Параметр **scope** может принимать указанные ниже значения. Это необязательный параметр. Если параметр **scope** не указан, создается ссылка с максимальными доступными разрешениями.

| Значение типа     | Описание                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | Создает доступную всем ссылку на элемент. Администратор клиента может отключить ссылки, не требующие проверки подлинности.                 |
| `organization` | Создает ссылку на элемент, доступную в организации. Область организации для ссылок недоступна в случае личных учетных записей OneDrive. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает в теле отклика один ресурс [Permission](../resources/permission.md), представляющий запрашиваемое разрешение для ссылки совместного доступа.

Для начала служба проверяет текущие разрешения на наличие значения **type**, подходящего для приложения, совершающего вызов.

Если для элемента создается новая ссылка совместного доступа, возвращается код отклика `201 Created`, а если возвращается существующая ссылка — код `200 OK`.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a>Отклик

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a>Создание ссылок с возможностью общего доступа в компании

OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании. Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующего клиента. Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a>HTTP-отклик

Если для элемента создается новая ссылка совместного доступа, возвращается код отклика `201 Created`, а если возвращается существующая ссылка — код `200 OK`.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a>Встроенные ссылки

При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.

**Примечание.** Встроенные ссылки поддерживаются только в ресурсах [Drive](../resources/drive.md), в которых для свойства **driveType** задано значение `personal`.

## <a name="remarks"></a>Заметки

* Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.
* Ссылки отображаются в разрешениях на совместное использование для элемента и могут быть удалены владельцем элемента.
* Они всегда указывают на текущую версию элемента, если он не был извлечен (только в SharePoint).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
