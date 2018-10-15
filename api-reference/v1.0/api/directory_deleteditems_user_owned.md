# <a name="list-deleted-items-owned-by-a-user"></a>**Список удаленных элементов, принадлежащих пользователю**

Извлечение списка недавно удаленных элементов, принадлежащих указанному пользователю.  

В настоящее время функция получения списка удаленных элементов поддерживается только для ресурсов группы ([group](../resources/group.md)), принадлежащих пользователю.

Это служебное действие, и, следовательно, оно не поддерживает разбиение на страницы.  Этот API возвращает до 1 000 удаленных объектов пользователя, отсортированных по идентификатору.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| --- | --- |
| Делегированные (рабочая или учебная учетная запись) | Group.Read.All, Group.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) |  Не поддерживается. |
| Для приложений | Group.Read.All, Group.ReadWrite.All  |

## <a name="http-request"></a>HTTP-запрос

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| ------------- | ------------------------- |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

В тексту запроса необходимо указать следующие параметры:

| Параметр    | Тип |Описание|
|:---------------|:--------|:----------|
|userId|String (строка)|Идентификатор владельца.|
|type|String (строка)|Тип объектов, принадлежащих пользователю, которые необходимо вернуть; `Group` — единственное поддерживаемое значение в настоящее время.|


## <a name="response"></a>Ответ

В случае успеха возвращаются коды ответа `200 OK`; объект ответа включает свойства [directory (удаленные элементы)](../resources/directory.md).

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>Ответ

Ниже приведен пример отклика. Примечание: этот объект отклика может быть усечен для краткости. Все поддерживаемые свойства возвращаются из фактических вызовов.

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


