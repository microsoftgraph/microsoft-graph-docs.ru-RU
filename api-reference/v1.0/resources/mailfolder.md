---
title: Тип ресурса mailFolder
description: Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a1ab83dfa3e3da64935a8c3976f12ffd1faf2e3c
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629387"
---
# <a name="mailfolder-resource-type"></a>Тип ресурса mailFolder

Пространство имен: microsoft.graph

Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/mailfolder-delta.md).

**Известные имена папок**

Outlook создает определенные папки для пользователей по умолчанию. Для удобства вместо значения **id** для доступа к папкам можно использовать известные имена папок из таблицы ниже. Например, вы можете получить папку черновиков, использовав ее известное имя со следующим запросом.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Известные имена поддерживаются вне зависимости от языкового стандарта почтового ящика пользователя, поэтому указанный выше запрос всегда возвращает папку черновиков пользователя, независимо от ее имени.

| Известное имя папки | Описание |
|:-----------------------|:------------|
| archive | Архивная папка, в которую отправляются сообщения при использовании функции архивации одним щелчком в клиентах Outlook, поддерживающих ее. **Примечание.** Она отличается от функции архивного почтового ящика Exchange Online. |
| clutter | Папка "Несрочные", в которую перемещаются сообщения низкой важности при использовании функции "Несрочные". |
| conflicts | Папка, содержащая конфликтующие элементы почтового ящика. |
| conversationhistory | Папка, в которой Skype сохраняет беседы при обмене мгновенными сообщениями (если Skype настроен для этого). |
| deleteditems | Папка, в которую перемещаются элементы при их удалении. |
| drafts | Папка, содержащая неотправленные сообщения. |
| inbox | Папка "Входящие". |
| junkemail | Папка нежелательной почты. |
| localfailures | Папка, содержащая элементы, существующие в локальном клиенте, но которые нельзя отправить на сервер. |
| msgfolderroot | Папка "Корневой уровень хранилища". Эта папка является родительской для папок, отображаемых в обычных почтовых клиентах, например в папке "Входящие". |
| outbox | Папка "Исходящие". |
| recoverableitemsdeletions | Папка, содержащая обратимо удаленные элементы: удаленные из папки "Удаленные" или путем нажатия клавиш SHIFT+DELETE в Outlook. Эта папка не отображается в почтовых клиентах Outlook, но пользователи могут взаимодействовать с ней с помощью функции **Восстановить удаленные элементы с сервера** в Outlook или Outlook в Интернете. |
| scheduled | Папка, содержащая сообщения, запланированные для повторного отображения в папке "Входящие" с помощью функции "Расписание" в Outlook для iOS. |
| searchfolders | Родительская папка для всех папок поиска, определенных в почтовом ящике пользователя. |
| sentitems | Папка "Отправленные". |
| serverfailures | Папка, содержащая элементы, существующие на сервере, но которые нельзя синхронизировать с локальным клиентом. |
| syncissues | Папка, содержащая журналы синхронизации, созданные в Outlook. |

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
|[Список объектов mailFolder](../api/user-list-mailfolders.md) | Коллекция [mailFolder](mailfolder.md)|Получение всех папок почты в указанном почтовом ящике пользователя, включая все папки поиска почты.|
|[Получение объекта mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |Чтение свойств и связей объекта mailFolder.|
|[Создание объекта mailFolder](../api/user-post-mailfolders.md) |[mailFolder](mailfolder.md)| Создание папки почты в корневой папке почтового ящика пользователя.|
|[Вывод списка объектов childFolder](../api/mailfolder-list-childfolders.md) |Коллекция [MailFolder](mailfolder.md)| Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.|
|[Создание объекта childFolder](../api/mailfolder-post-childfolders.md) |[mailFolder](mailfolder.md)| Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolder.|
|[Создание сообщения](../api/mailfolder-post-messages.md) |[Message](message.md)| Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.|
|[Вывод списка сообщений](../api/mailfolder-list-messages.md) |Коллекция объектов [Message](message.md)| Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.|
|[Обновление](../api/mailfolder-update.md) | [mailFolder](mailfolder.md)|Обновление указанного объекта mailFolder. |
|[Удаление](../api/mailfolder-delete.md) | Нет |Удаление указанного объекта mailFolder. |
|[copy](../api/mailfolder-copy.md)|[MailFolder](mailfolder.md)|Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.|
|[delta](../api/mailfolder-delta.md)|Коллекция [mailFolder](mailfolder.md)|Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.|
|[move](../api/mailfolder-move.md)|[MailFolder](mailfolder.md)|Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.|
|**Расширенные свойства**| | |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[mailFolder](mailfolder.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.   |
|[Получение элемента mailFolder с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [mailFolder](mailfolder.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.  |
|[Получение элемента mailFolder с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|childFolderCount|Int32|Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.|
|displayName|Строка|Отображаемое имя элемента mailFolder.|
|id|Строка|Уникальный идентификатор элемента mailFolder.|
|isHidden|Логический|Указывает, скрыт ли объект mailFolder. Это свойство можно установить только при создании папки. Дополнительные сведения см. в разделе [Скрытые папки почты](#hidden-mail-folders).|
|parentFolderId|Строка|Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.|
|totalItemCount|Int32|Количество элементов в элементе mailFolder.|
|unreadItemCount|Int32|Количество элементов, помеченных как непрочитанные, в элементе mailFolder.|

**Эффективный доступ к сведениям о количестве элементов**

Используя такие свойства папки, как `TotalItemCount` и `UnreadItemCount`, можно удобно вычислять количество прочитанных элементов в папке.
Благодаря им можно не использовать запросы (например, указанный ниже), выполнение которых может привести к значительным задержкам.

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Папки почты в Outlook могут содержать элементы нескольких типов, например, папка "Входящие" может содержать элементы приглашений на собрания, не связанные с почтовыми элементами. Свойства `TotalItemCount` и `UnreadItemCount` включают элементы из папки почты вне зависимости от их типов.

### <a name="hidden-mail-folders"></a>Скрытые папки почты
Значение свойства `isHidden` по умолчанию: `false`. Вы можете задать **isHidden** только один раз при [создании объекта mailFolder](../api/user-post-mailfolders.md). Обновление свойства с помощью операции PATCH невозможно. Чтобы изменить свойство **isHidden** папки, удалите существующую папку и создайте новую с нужным значением.

Скрытые папки почты поддерживают все операции, поддерживаемые обычной почтовой папкой.

По умолчанию при [перечислении объектов mailFolder](../api/user-list-mailfolders.md) возвращаются только не скрытые папки почты. Чтобы включить скрытые папки почты в отклик, используйте параметр запроса `includeHiddenFolders=true`. Затем используйте свойство **isHidden**, чтобы определить, скрыта ли папка почты. 

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
  "isHidden": false,
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview)
- [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

