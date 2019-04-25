---
title: Тип ресурса mailFolder
description: Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1cd48c866ea6384aa18631732065380e898b8bf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547132"
---
# <a name="mailfolder-resource-type"></a>Тип ресурса mailFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/mailfolder-delta.md).

**Стандартные имена папок**

Outlook создает определенные папки для пользователей по умолчанию. Вместо того чтобы использовать значение **идентификатора** соответствующей папки для удобства, вы можете использовать известные имена папок из приведенной ниже таблицы при доступе к этим папкам. Например, вы можете получить папку черновиков с помощью известного имени с помощью следующего запроса.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Хорошо известные имена работают независимо от языкового стандарта почтового ящика пользователя, поэтому вышеприведенный запрос всегда возвращает папку черновиков пользователя независимо от того, как она названа.

| Известное имя папки | Описание |
|:-----------------------|:------------|
| сохранении | Сообщения архивных папок отправляются при использовании компонента архива Оне_кликк в клиентах Outlook, поддерживающих эту службу. **Примечание:** это не то же самое, что функция архивного почтового ящика в Exchange Online. |
| папк | Сообщения с минимальным приоритетом перемещаются в папку "несрочные" при использовании функции "неСрочные". |
| речи | Папка, содержащая конфликтующие элементы в почтовом ящике. |
| conversationhistory | Папка, в которой Skype сохраняет обмен МГНОВЕНными СООБЩЕНИЯми (если для этого настроен Skype). |
| deleteditems | Элементы папки перемещаются в то время, когда они удаляются. |
| "Черновики" | Папка, содержащая неотправленные сообщения. |
| папке Входящие " | Папка "Входящие". |
| жункемаил | Папка нежелательной почты. |
| локалфаилурес | Папка, содержащая элементы, которые существуют в локальном клиенте, но их не удалось отправить на сервер. |
| мсгфолдеррут | Папка "Верхняя часть информационного хранилища". Эта папка является родительской папкой для папок, отображаемых в обычных почтовых клиентах, например в папке "Входящие". |
| ходящие | Папка "Исходящие". |
| рековераблеитемсделетионс | Папка, содержащая обратимо удаленные элементы: удалена из папки "Удаленные" или с помощью сочетания клавиш Shift + Delete в Outlook. Эта папка не видна в почтовом клиенте Outlook, но конечные пользователи могут взаимодействовать с ним с помощью функции **восстановления удаленных элементов с сервера** в Outlook или Outlook в Интернете. |
| календар | Папка, содержащая сообщения, которые запланировано повторно отображать в папке "Входящие" с помощью функции расписания в Outlook для iOS. |
| searchfolders | Родительская папка для всех папок поиска, определенных в почтовом ящике пользователя. |
| sentitems | Папка "Отправленные". |
| серверфаилурес | Папка, содержащая элементы, которые существуют на сервере, но не может быть синхронизирована с локальным клиентом. |
| синЦиссуес | Папка, содержащая журналы синхронизации, созданные в Outlook. |

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
|[Получение объекта mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md); |Чтение свойств и связей объекта mailFolder.|
|[Создание объекта MailFolder](../api/mailfolder-post-childfolders.md) |[mailFolder](mailfolder.md);| Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolders.|
|[Вывод списка объектов childFolder](../api/mailfolder-list-childfolders.md) |Коллекция [mailFolder](mailfolder.md)| Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.|
|[Создание сообщения](../api/mailfolder-post-messages.md) |[message](message.md)| Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.|
|[Список сообщений](../api/mailfolder-list-messages.md) |Коллекция [message](message.md)| Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.|
|[Обновление](../api/mailfolder-update.md) | [mailFolder](mailfolder.md);|Обновление указанного объекта mailFolder. |
|[Удаление](../api/mailfolder-delete.md) | Нет |Удаление указанного объекта mailFolder. |
|[copy](../api/mailfolder-copy.md)|[mailFolder](mailfolder.md);|Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.|
|[delta](../api/mailfolder-delta.md)|Коллекция [mailFolder](mailfolder.md)|Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.|
|[move](../api/mailfolder-move.md)|[mailFolder](mailfolder.md);|Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.|
|**Расширенные свойства**| | |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[mailFolder](mailfolder.md);  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.   |
|[Получение элемента mailFolder с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md); | Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [mailFolder](mailfolder.md); | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.  |
|[Получение элемента mailFolder с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|childFolderCount|Int32|Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.|
|displayName|Строка|Отображаемое имя элемента mailFolder.|
|id|Строка|Уникальный идентификатор элемента mailFolder.|
|parentFolderId|String|Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.|
|totalItemCount|Int32|Количество элементов в элементе mailFolder.|
|unreadItemCount|Int32|Количество элементов, помеченных как непрочитанные, в элементе mailFolder.|
|wellKnownName|String|Хорошо известное имя папки для папки. Ниже перечислены возможные значения. Это свойство задается только для папок по умолчанию, создаваемых в Outlook. Для других папок это свойство имеет **значение NULL**.|

**Эффективный доступ к сведениям о количестве элементов**

Свойства `TotalItemCount` папки `UnreadItemCount` и свойства папки позволяют удобно вычислить количество прочитанных элементов в папке.
Благодаря им можно не использовать запросы (например, указанный ниже), выполнение которых может привести к значительным задержкам.

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

ПоЧтовые папки в Outlook могут содержать более одного типа элементов, например, папка "Входящие" может содержать элементы приглашения на собрания, которые отличаются от элементов почты. `TotalItemCount`и `UnreadItemCount` включать элементы в папку почты независимо от их типов элементов.

## <a name="relationships"></a>Связи

| Отношение | Тип | Описание |
|:-------------|:-----|:------------|
|childFolders|Коллекция объектов [MailFolder](mailfolder.md)|Коллекция дочерних папок в элементе mailFolder.|
|messageRules | Коллекция [messageRule](messagerule.md) | Коллекция правил, которые применяются к папке пользователя "Входящие". |
|messages|Коллекция [Message](message.md)|Коллекция сообщений в элементе mailFolder.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для элемента mailFolder. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для элемента mailFolder. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "wellKnownName": "string",
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью запроса изменений](/graph/delta-query-overview)
- [Получение добавочных изменений сообщений в папке](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
