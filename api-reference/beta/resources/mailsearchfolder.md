---
title: Тип ресурса Маилсеарчфолдер
description: Маилсеарчфолдер — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска. Маилсеарчфолдер наследуется от mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ce4abccab636d8e73f4f423b4270e8804a4634eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522822"
---
# <a name="mailsearchfolder-resource-type"></a>Тип ресурса Маилсеарчфолдер

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Маилсеарчфолдер** — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска. **маилсеарчфолдер** наследуется от [mailFolder](mailfolder.md). Папки поиска можно создавать в любой папке почтового ящика Exchange Online пользователя. Однако для отображения папки поиска в Outlook, Outlook для Интернета или Outlook Live необходимо создать папку в папке **веллкновнфолдернаме. SearchFolders** . 

## <a name="search-folder-lifecycle"></a>Жизненный цикл папок поиска

Папки поиска, созданные приложением, могут быть удалены в Exchange Online по одной из следующих причин:

1.  Срок действия папок поиска истечет через 45 дней без использования. 
2.  Количество папок поиска, которые могут быть созданы для каждой исходной папки, ограничено. При нарушении этого ограничения старые папки поиска удаляются, чтобы сделать новые. 

При удалении папки поиска приложение должно создать новый ресурс папки поиска и использовать тот же ресурс.


## <a name="methods"></a>Методы

| Метод | Возвращаемый тип  | Описание |
|:---------------|:--------|:----------|
| [Создание папки поиска](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | Создайте папку поиска в почтовом ящике этого пользователя. |
| [Список папок поиска](../api/mailfolder-list-childfolders.md) | Коллекция [mailFolder](mailfolder.md) | Перечислите все папки в почтовом ящике этого пользователя, в том числе папки поиска. |
| [Получение папки поиска](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | Получение указанной папки поиска. |
| [Обновление папки поиска](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | Обновление указанной папки поиска. |
| [Удаление папки поиска](../api/mailfolder-delete.md) | Нет | Удаление указанной папки поиска. |
| [Перечисление всех сообщений в папке поиска](../api/mailfolder-list-messages.md) | Коллекция [message](message.md) | Перечисление всех сообщений в указанной папке поиска. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| Поддержка | Логический | Указывает, является ли папка поиска редактируемой с помощью REST API. |
| инклуденестедфолдерс | Логический | Указывает, как должна проходить иерархия папок почтовых ящиков в поиске. `true`означает, что необходимо выполнить глубокий поиск, чтобы включить дочерние папки в иерархию каждой папки, явно указанной в **саурцефолдеридс**. `false`означает неглубокий Поиск только тех папок, которые явно указаны в **саурцефолдеридс**. |
| саурцефолдеридс | Коллекция String | Папки почтовых ящиков, которые должны быть mined. |
| филтеркуери | String | Запрос OData для фильтрации сообщений. |

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
