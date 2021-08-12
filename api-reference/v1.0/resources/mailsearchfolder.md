---
title: тип ресурса mailSearchFolder
description: MailSearchFolder — это виртуальная папка в почтовом ящике пользователя, которая содержит все элементы электронной почты, совпадающие с указанными критериями поиска. mailSearchFolder наследует от mailFolder.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 85d64d007f8a74f1475156a48dd3c281c591678838ca19f4644b1df3eec4c038
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141492"
---
# <a name="mailsearchfolder-resource-type"></a>тип ресурса mailSearchFolder

Пространство имен: microsoft.graph

**MailSearchFolder** — это виртуальная папка в почтовом ящике пользователя, которая содержит все элементы электронной почты, совпадающие с указанными критериями поиска. **mailSearchFolder** наследует от [mailFolder](mailfolder.md). Папки поиска можно создавать в любой папке в почтовом Exchange Online пользователя. Однако для того, чтобы папка поиска Outlook, Outlook веб Outlook Live, папка должна быть создана в папке **WellKnownFolderName.SearchFolders.** 

## <a name="search-folder-lifecycle"></a>Жизненный цикл папки поиска

Папки поиска, созданные вашим приложением, могут быть удалены Exchange Online по одной из следующих причин:

1.  Срок действия папки поиска истекает через 45 дней без использования. 
2.  Существует ограничение на количество папок поиска, которые можно создать в одной папке источника. При нарушении этого ограничения старые папки поиска удаляются, чтобы уложиться в новые. 

При удалении папки поиска приложение должно создать новый ресурс папки поиска и использовать то же самое.


## <a name="methods"></a>Методы

| Метод | Возвращаемый тип  | Описание |
|:---------------|:--------|:----------|
| [Создание папки поиска](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | Создайте папку поиска в почтовом ящике этого пользователя. |
| [Папки поиска списка](../api/mailfolder-list-childfolders.md) | Коллекция [mailFolder](mailfolder.md) | Список всех папок в почтовом ящике этого пользователя, включая папки поиска. |
| [Получить папку поиска](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | Получите указанную папку поиска. |
| [Обновление папки поиска](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | Обновление указанной папки поиска. |
| [Удаление папки поиска](../api/mailfolder-delete.md) | Нет | Удаление указанной папки поиска. |
| [Список всех сообщений в папке поиска](../api/mailfolder-list-messages.md) | Коллекция [message](message.md) | Список всех сообщений в указанной папке поиска. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| isSupported | Логический | Указывает, является ли папка поиска редактируемой с помощью API REST. |
| includeNestedFolders | Логический | Указывает, как должна проходить иерархия папок почтовых ящиков в поиске. `true` означает, что следует сделать глубокий поиск, чтобы включить детские папки в иерархию каждой папки, явно указанной в **sourceFolderIds**. `false`означает неглубокий поиск только каждой из папок, явно указанных в **sourceFolderIds.** |
| sourceFolderIds | Коллекция строк | Папки почтовых ящиков, которые необходимо добыть. |
| filterQuery | String | Запрос OData для фильтрации сообщений. |

## <a name="json-representation"></a>Представление JSON

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

