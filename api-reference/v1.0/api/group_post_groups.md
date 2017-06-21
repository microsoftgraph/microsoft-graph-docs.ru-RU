# <a name="create-group"></a>Создание группы

Используйте этот API, чтобы создать группу согласно инструкциям в тексте запроса. Можно создать один из трех типов групп:

* Группа Office 365 (единая группа)
* Динамическая группа
* Группа безопасности

> **Примечание.** Несмотря на то что Microsoft Teams создан на основе групп Office 365, в настоящее время нельзя создать группу через этот API. Вы можете использовать другие API групп для управления группой, созданной в Microsoft Teams.

## <a name="prerequisites"></a>Необходимые условия
Для применения этого API требуется следующая **область**: _Group.ReadWrite.All_ 
## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В таблице ниже представлены свойства ресурса [group](../resources/group.md), который необходимо указать по крайней мере при создании группы. 

| Свойство | Тип | Описание|
|:---------------|:--------|:----------|
| displayName | string | Имя, которое следует отобразить в адресной книге для группы. |
| mailEnabled | boolean | Устанавливает значение **true** для групп с включенной поддержкой почты. Установите значение **true** при создании группы Office 365. При создании динамической группы или группы безопасности установите для этого свойства значение **false**.|
| mailNickname | string | Почтовый псевдоним для группы. |
| securityEnabled | boolean | Устанавливает значение **true** для групп безопасности. При создании динамической группы или группы безопасности установите для этого свойства значение **true**. Устанавливает значение **false** при создании группы Office 365. |

При создании динамической группы или группы Office 365 укажите свойство **groupTypes**, как описано ниже.

| Тип группы | Свойство **groupTypes** |
|:--------------|:------------------------|
| Office 365 (как единая группа)| "Unified" | 
| Динамическая группа | "DynamicMembership" | 
| Система безопасности | Не следует устанавливать. | 

При необходимости укажите другие записываемые свойства для своей группы. Дополнительные сведения см. в таблице свойств ресурса [group](../resources/group.md).

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201, Created` и объект [group](../resources/group.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ознакомьтесь с примером запроса, создающего группу Office 365.
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будет возвращено больше свойств.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
