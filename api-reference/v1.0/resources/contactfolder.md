# <a name="contactfolder-resource-type"></a>Тип ресурса contactFolder

Папка, содержащая контакты.

В этом ресурсе возможно использование [запроса изменений](../../../concepts/delta_query_overview.md) для отслеживания добавочных дополнений, удалений и обновлений благодаря функции [delta](../api/contactfolder_delta.md).


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение contactFolder](../api/contactfolder_get.md) | [contactFolder](contactfolder.md) |Получение папки с контактами с помощью идентификатора папки контактов.|
|[Обновление](../api/contactfolder_update.md) | [contactFolder](contactfolder.md) |Обновление объекта contactFolder. |
|[Удаление](../api/contactfolder_delete.md) | Нет |Удаление объекта contactFolder. |
|[Список экземпляров childFolders](../api/contactfolder_list_childfolders.md) |Коллекция [ContactFolder](contactfolder.md)| Получение коллекции дочерних папок для указанной папки с контактами.|
|[Создание дочернего элемента contactFolder](../api/contactfolder_post_childfolders.md) |[ContactFolder](contactfolder.md)| Создание дочернего элемента contactFolder для указанной папки.|
|[delta](../api/contact_delta.md)|Коллекция [contact](contact.md)| Получение набора папок контактов, которые были добавлены в почтовый ящик пользователя или удалены из него.|
|[Список контактов в папке](../api/contactfolder_list_contacts.md) |Коллекция [contact](contact.md)| Получение коллекции контактов из стандартной папки с контактами для пользователя, выполнившего вход (`.../me/contacts`), или из указанной папки с контактами.|
|[Создание контакта в папке](../api/contactfolder_post_contacts.md) |[Contact](contact.md)| Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.|
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[contactFolder](contactFolder.md)  |Создание одного или несколько расширенных свойств с одним значением в новом или существующем экземпляре contactFolder.   |
|[Получение contactFolder с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty_get.md)  | [contactFolder](contactFolder.md) | Получение экземпляров contactFolder, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [contactFolder](contactFolder.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем экземпляре contactFolder.  |
|[Получение contactFolder с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty_get.md)  | [contactFolder](contactFolder.md) | Получение экземпляра contactFolder, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|Строка|Отображаемое имя папки.|
|id|Строка|Уникальный идентификатор папки с контактами. Только для чтения.|
|parentFolderId|Строка|Идентификатор родительской папки для папки.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|childFolders|Коллекция [ContactFolder](contactfolder.md)|Коллекция дочерних папок в папке. Свойство навигации. Только для чтения. Допускается значение null.|
|contacts|Коллекция [contact](contact.md)|Контакты в папке. Свойство навигации. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для contactFolder. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для contactFolder. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.contactFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "navigability": "single",
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string"
}

```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью разностного запроса](../../../concepts/delta_query_overview.md)
- [Получение добавочных изменений сообщений в папке](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
