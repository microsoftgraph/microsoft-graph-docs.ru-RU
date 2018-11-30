---
title: Тип ресурса mailSearchFolder
description: MailSearchFolder является виртуальной папки в почтовом ящике пользователя, который содержит все элементы электронной почты, соответствующие заданным критериям поиска. mailSearchFolder наследует от mailFolder.
ms.openlocfilehash: abce7c86e44fcee98042aecf753f0fdf4172365e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079876"
---
# <a name="mailsearchfolder-resource-type"></a>Тип ресурса mailSearchFolder

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

MailSearchFolder является виртуальной папки в почтовом ящике пользователя, который содержит все элементы электронной почты, соответствующие заданным критериям поиска. mailSearchFolder наследует от [mailFolder](mailfolder.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип  | Описание |
|:---------------|:--------|:----------|
| [Создание папки поиска](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | Создание папки поиска в этом почтовом ящике пользователя. |
| [Список папок поиска](../api/mailfolder-list-childfolders.md) | Коллекция [mailFolder](mailfolder.md) | Список всех папок в этом почтовом ящике пользователя, включая папки поиска. |
| [Получение папки поиска](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | Получение папки поиска. |
| [Изменение папки поиска](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | Обновление папки поиска. |
| [Удаление папки поиска](../api/mailfolder-delete.md) | Нет | Удаление папки поиска. |
| [Список всех сообщений в папке поиска](../api/mailfolder-list-messages.md) | Коллекция объектов [message](message.md) | Список всех сообщений в папке поиска. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Description |
|:---------------|:--------|:----------|
| isSupported | Логический | Указывает, является ли папки поиска редактирования с помощью API-интерфейсы REST. |
| includeNestedFolders | Логический | Указывает, как должен выполняться иерархии папок почтового ящика. `true`означает, что глубокого поиска должны быть в то время как `false` означает, что следует частичного поиска. |
| sourceFolderIDs | Коллекция String | Папки почтовых ящиков, которые должны быть получены. |
| filterQuery | String | Запросов OData для фильтрации сообщений. |

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
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
