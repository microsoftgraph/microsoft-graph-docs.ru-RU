---
title: Тип ресурса mailSearchFolder
description: MailSearchFolder является виртуальной папки в почтовом ящике пользователя, который содержит все элементы электронной почты, соответствующие заданным критериям поиска. mailSearchFolder наследует от mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520986"
---
# <a name="mailsearchfolder-resource-type"></a>Тип ресурса mailSearchFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| isSupported | Логическое | Указывает, является ли папки поиска редактирования с помощью API-интерфейсы REST. |
| includeNestedFolders | Логическое | Указывает, как должен выполняться иерархии папок почтового ящика. `true`означает, что глубокого поиска должны быть в то время как `false` означает, что следует частичного поиска. |
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
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailsearchfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
