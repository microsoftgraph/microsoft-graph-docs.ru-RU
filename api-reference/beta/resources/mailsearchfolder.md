---
title: Тип ресурса mailSearchFolder
description: MailSearchFolder — это виртуальная папка в почтовом ящике пользователя, которая содержит все элементы электронной почты, которые соответствуют указанным условиям поиска. mailSearchFolder наследуется от mailFolder.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6740d6bac12ca02938c24f6e36dc48b0ab3a316f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129851"
---
# <a name="mailsearchfolder-resource-type"></a>Тип ресурса mailSearchFolder

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**MailSearchFolder** — это виртуальная папка в почтовом ящике пользователя, которая содержит все элементы электронной почты, которые соответствуют указанным условиям поиска. **mailSearchFolder** наследуется от [mailFolder.](mailfolder.md) Папки поиска можно создавать в любой папке в почтовом ящике пользователя Exchange Online. Однако чтобы папка поиска появлялись в Outlook, Outlook в Интернете или Outlook Live, ее необходимо создать в папке **WellKnownFolderName.SearchFolders.** 

## <a name="search-folder-lifecycle"></a>Жизненный цикл папки поиска

Exchange Online может удалить папки поиска, созданные приложением, по одной из следующих причин:

1.  Срок действия папок поиска истекает через 45 дней без использования. 
2.  Количество папок поиска, которые можно создать для одной папки источника, ограничивается. При нарушении этого ограничения старые папки поиска удаляются для укладки новых. 

При удалении папки поиска приложение должно создать новый ресурс папки поиска и использовать то же самое.


## <a name="methods"></a>Методы

| Метод | Возвращаемый тип  | Описание |
|:---------------|:--------|:----------|
| [Создание папки поиска](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | Создайте папку поиска в почтовом ящике этого пользователя. |
| [Список папок поиска](../api/mailfolder-list-childfolders.md) | Коллекция [mailFolder](mailfolder.md) | Список всех папок в почтовом ящике этого пользователя, включая папки поиска. |
| [Получить папку поиска](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | Получите указанную папку поиска. |
| [Обновление папки поиска](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | Обновим указанную папку поиска. |
| [Удаление папки поиска](../api/mailfolder-delete.md) | Нет | Удалите указанную папку поиска. |
| [Список всех сообщений в папке поиска](../api/mailfolder-list-messages.md) | Коллекция [message](message.md) | Список всех сообщений в указанной папке поиска. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| isSupported | Boolean | Указывает, можно ли редактировать папку поиска с помощью REST API. |
| includeNestedFolders | Boolean | Указывает, как должна проходить иерархия папок почтового ящика в поиске. `true`означает, что следует глубоко искать, чтобы включить в иерархию каждой папки, явно указанной в **sourceFolderIds.** `false`означает неглубокий поиск только каждой папки, явно указанной в **sourceFolderIds.** |
| sourceFolderIds | Коллекция объектов string | Папки почтового ящика, которые необходимо миновать. |
| filterQuery | Строка | Запрос OData для фильтрации сообщений. |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


