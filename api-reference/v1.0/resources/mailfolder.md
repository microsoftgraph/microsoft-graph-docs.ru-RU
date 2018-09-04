# <a name="mailfolder-resource-type"></a>Тип ресурса mailFolder

Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.

Этот ресурс поддерживает применение [разностного запроса](../../../concepts/delta_query_overview.md) для отслеживания вносимых добавлений, удалений и обновлений при помощи функции [delta](../api/mailfolder_delta.md).

**Стандартные имена папок**

Некоторые папки для пользователей создаются Outlook по умолчанию. Для удобства, при доступе к этим папкам вместо соответствующего значения **id** папки можно использовать стандартные имена папок, взятые из приведенной ниже таблицы. Так, к примеру, для получения доступа к папке «Черновики» при помощи ее широко известного имени может использоваться следующий запрос.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Широко известные имена работают независимо от языкового стандарта, применяемого для почтового ящика пользователя, и приведенный выше запрос всегда будет возвращать пользовательскую папку «Черновики», независимо от того, какое имя ей присвоено.

| Широко известное имя папки | Описание |
|:-----------------------|:------------|
| archive | Отправка сообщений в папку архива осуществляется при использовании функции архивации One_Click в тех клиентах Outlook, которые ее поддерживают. **Примечание.** Эта функция не является аналогом функции Archive Mailbox, доступной в Exchange online. |
| clutter | Сообщения с низким приоритетом перемещаются в папку «Несрочные» при использовании функции Clutter. |
| conflicts | В этой папке, содержатся конфликтующие элементы, имеющиеся в почтовом ящике. |
| conversationhistory | В этой папке Skype сохраняет текстовые беседы (при соответствующих настройках). |
| deleteditems | Перемещение отдельных элементов в эту папку производится при их удалении. |
| drafts | Папка «Черновики», содержащая неотправленные сообщения. |
| inbox | Папка «Входящие». |
| junkemail | Папка нежелательной почты. |
| localfailures | Папка, которые содержит элементы, имеющиеся на локальном клиенте, но не загруженные на сервер. |
| msgfolderroot | Папка «Корневого уровня хранилища». Эта папка является родительской папкой для папок, отображаемых в обычных почтовых клиентах, таких как папка «Входящие». |
| outbox | Папка «Исходящие» |
| recoverableitemsdeletions | Папка, которая содержит элементы, удаленные с возможностью восстановления: элементы, удаленные из папки «Удаленные», либо элементы, удаленные нажатием на клавиши shift+delete в Outlook. Эта папка не отображается ни в одном из почтовых клиентов Outlook, но конечные пользователи могут взаимодействовать с ней при помощи функции **Восстановить удаленные элементы с сервера**, доступной в Outlook или Outlook в Интернете. |
| scheduled | Папка, содержащая сообщения, повторное помещение которых в папку «Входящие» запланировано с помощью функции «Планирование» в Outlook для iOS. |
| searchfolders | Родительская папка для всех папок поиска, определенных в почтовом ящике пользователя. |
| sentitems | Папка "Отправленные" |
| serverfailures | Папка, которая содержит элементы, имеющиеся на сервере, но не синхронизированные с локальным клиентом. |
| syncissues | Папка, содержащая созданные Outlook журналы синхронизации. |

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
|[Получение объекта mailFolder](../api/mailfolder_get.md) | [mailFolder](mailfolder.md) |Чтение свойств и связей объекта mailFolder.|
|[Создание объекта MailFolder](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolders.|
|[Вывод списка объектов childFolder](../api/mailfolder_list_childfolders.md) |Коллекция [MailFolder](mailfolder.md)| Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.|
|[Создание сообщения](../api/mailfolder_post_messages.md) |[Message](message.md)| Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.|
|[Вывод списка сообщений](../api/mailfolder_list_messages.md) |Коллекция объектов [Message](message.md)| Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.|
|[Обновление](../api/mailfolder_update.md) | [mailFolder](mailfolder.md)|Обновление указанного объекта mailFolder. |
|[Удаление](../api/mailfolder_delete.md) | Нет |Удаление указанного объекта mailFolder. |
|[copy](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)|Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.|
|[delta](../api/mailfolder_delta.md)|Коллекция [mailFolder](mailfolder.md)|Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.|
|[move](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)|Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.   |
|[Получение элемента mailFolder с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.  |
|[Получение элемента mailFolder с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|childFolderCount|Int32|Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.|
|displayName|Строка|Отображаемое имя элемента mailFolder.|
|id|Строка|Уникальный идентификатор mailFolder.|
|parentFolderId|Строка|Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.|
|totalItemCount|Int32|Количество элементов в элементе mailFolder.|
|unreadItemCount|Int32|Количество элементов, помеченных как непрочитанные, в элементе mailFolder.|

**Эффективный доступ к сведениям о количестве элементов**

Свойства `TotalItemCount` и `UnreadItemCount` папки позволяют с легкостью определить количество содержащихся в ней прочитанных элементов.
Они позволяют избежать подачи запросов, подобных тем, которые приводятся ниже, и которые могут вызывать значительную задержку:

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Папки почты в Outlook могут содержать элементы нескольких типов, например, в папке «Входящие» могут находиться элементы запроса на проведение собрания, отличающиеся от почтовых элементов. `TotalItemCount` TotalItemCount и UnreadItemCount`UnreadItemCount`  позволяют включать элементы в папку почты независимо от их типа.

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:-------------|:-----|:------------|
|childFolders|Коллекция объектов [MailFolder](mailfolder.md)|Коллекция дочерних папок в элементе mailFolder.|
|messageRules | Коллекция [messageRule](messagerule.md) | Коллекция правил, которые применяются к папке пользователя "Входящие". |
|messages|Коллекция объектов [Message](message.md)|Коллекция сообщений в элементе mailFolder.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для элемента mailFolder. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для элемента mailFolder. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью разностного запроса](../../../concepts/delta_query_overview.md)
- [Получение добавочных изменений сообщений в папке](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
