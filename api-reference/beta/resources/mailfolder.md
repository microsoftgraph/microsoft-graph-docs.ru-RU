---
title: Тип ресурса mailFolder
description: Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.
localization_priority: Normal
ms.openlocfilehash: a44819f0248e8d6e410e2c6bd57e727ae719b1d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881622"
---
# <a name="mailfolder-resource-type"></a>Тип ресурса mailFolder

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Почтовая папка в почтовом ящике пользователя, например "Входящие" или "Черновики". Почтовые папки могут содержать сообщения, другие элементы Outlook и дочерние почтовые папки.

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/mailfolder-delta.md).

**Имена папок хорошо известные**

Outlook создает определенные папки для пользователей по умолчанию. Вместо использования соответствующее значение **идентификатора** папки для удобства, можно использовать имена известных папок из приведенной ниже таблице при доступе к этих папок. Например можно получить папке "Черновики", с помощью имени известных с помощью следующего запроса.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Хорошо известные имена работать независимо от языкового стандарта из почтового ящика пользователя выше запрос всегда будет возвращать Папка «Черновики» пользователя независимо от того, как с именем.

| Имя хорошо известные папки | Описание |
|:-----------------------|:------------|
| архив | Сообщения папки архива отправляются при использовании функции архивации One_Click в клиентах Outlook, которые поддерживают его. **Примечание:** это не то же, что компонент архивного почтового ящика из Exchange online. |
| засорение | Сообщения с низким приоритетом папки засорение перемещаются при использовании функции беспорядок. |
| конфликтов | Папка, содержащая конфликтующих элементов в почтовом ящике. |
| conversationhistory | Папка, где Скайп сохраняет мгновенные сообщения (если Скайп настроен для этого). |
| deleteditems | Элементы папки перемещаются при удалении. |
| черновики | Папка, содержащая неотправленные сообщения. |
| папки «Входящие» | Папка "Входящие". |
| junkemail | В папку нежелательной почты. |
| localfailures | Папка, содержащая элементы, которые существуют на локальных клиентов, но не удалось загрузить на сервер. |
| msgfolderroot | Папка «Хранилища». Эта папка является родительской папки для папок, которые отображаются в обычном почтовых клиентах, таких как папки «Входящие». |
| Исходящие | Папка "Исходящие". |
| recoverableitemsdeletions | Папка, содержащая удаленные элементы: удален из папки «Удаленные», либо при нажатии клавиши shift + удаление в Outlook. Эта папка не отображается в любой клиент электронной почты Outlook, но конечные пользователи могут взаимодействовать с его посредством функции **Восстановить удаленные элементы с сервера** в Outlook или Outlook в Интернете. |
| запланировано | Папка, содержащая сообщения, которые планируется снова появится в папке "Входящие", с помощью функции расписание в Outlook для операций ввода-вывода. |
| searchfolders | Родительской папки для всех папок поиска, определенного в почтовом ящике пользователя. |
| папки "Отправленные" | Папке «Отправленные». |
| serverfailures | Папка, содержащая элементы, которые существуют на сервере, но не будет синхронизирована с локальных клиентских. |
| syncissues | Папка, содержащая синхронизации журналов, созданных в Outlook. |

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-------|:------------|:------------|
|[Получение объекта mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |Чтение свойств и связей объекта mailFolder.|
|[Создание объекта MailFolder](../api/mailfolder-post-childfolders.md) |[mailFolder](mailfolder.md)| Создание объекта mailFolder в текущем объекте путем публикации в коллекции элементов childFolders.|
|[Вывод списка объектов childFolder](../api/mailfolder-list-childfolders.md) |Коллекция [mailFolder](mailfolder.md)| Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.|
|[Создание сообщения](../api/mailfolder-post-messages.md) |[message](message.md)| Создание сообщения в текущем элементе mailFolder путем его публикации в коллекции сообщений.|
|[Вывод списка сообщений](../api/mailfolder-list-messages.md) |Коллекция [message](message.md)| Получение всех сообщений в почтовом ящике пользователя, вошедшего в систему, или в указанной папке почтового ящика.|
|[Обновление](../api/mailfolder-update.md) | [mailFolder](mailfolder.md)|Обновление указанного объекта mailFolder. |
|[Удаление](../api/mailfolder-delete.md) | Нет |Удаление указанного объекта mailFolder. |
|[copy](../api/mailfolder-copy.md)|[mailFolder](mailfolder.md)|Копирование элемента mailFolder и его содержимого в другой элемент mailFolder.|
|[delta](../api/mailfolder-delta.md)|Коллекция [mailFolder](mailfolder.md)|Получение набора папок почты, которые были добавлены в почтовый ящик пользователя или удалены из него.|
|[move](../api/mailfolder-move.md)|[mailFolder](mailfolder.md)|Перемещение элемента mailFolder и его содержимого в другой элемент mailFolder.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[mailFolder](mailfolder.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем элементе mailFolder.   |
|[Получение элемента mailFolder с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Получение элементов mailFolder, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [mailFolder](mailfolder.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем элементе mailFolder.  |
|[Получение элемента mailFolder с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Получение элемента mailFolder, который содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------|:-----|:------------|
|childFolderCount|Int32|Количество непосредственных дочерних элементов mailFolder в текущем элементе mailFolder.|
|displayName|Строка|Отображаемое имя элемента mailFolder.|
|id|Строка|Уникальный идентификатор mailFolder.|
|parentFolderId|Строка|Уникальный идентификатор родительского элемента mailFolder для элемента mailFolder.|
|totalItemCount|Int32|Количество элементов в элементе mailFolder.|
|unreadItemCount|Int32|Количество элементов, помеченных как непрочитанные, в элементе mailFolder.|
|wellKnownName|Строка|Хорошо известные папки имя папки. Возможные значения перечислены выше. Это свойство принимает значение только для папок по умолчанию, созданные в Outlook. Для других папок это свойство имеет **значение null**.|

**Эффективный доступ к сведениям о количестве элементов**

`TotalItemCount` И `UnreadItemCount` свойства папки позволяют легко создавать вычисления количества чтения элементов в папке.
Они позволяют предотвратить запросов, который может привести к значительным задержка следующим образом:

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Почтовые папки в Outlook может содержать несколько типов элементов, например, может содержать папки «Входящие» элементы запроса, которые отличаются от почтовых элементов собрания. `TotalItemCount`и `UnreadItemCount` включать элементы в папке почты независимо от их типов элементов.

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:-------------|:-----|:------------|
|childFolders|Коллекция объектов [MailFolder](mailfolder.md)|Коллекция дочерних папок в элементе mailFolder.|
|messageRules | Коллекция [messageRule](messagerule.md) | Коллекция правил, которые применяются к папке пользователя "Входящие". |
|messages|Коллекция объектов [Message](message.md)|Коллекция сообщений в элементе mailFolder.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для элемента mailFolder. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для элемента mailFolder. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

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
