---
title: Тип ресурса Маилсеарчфолдер
description: Маилсеарчфолдер — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска. Маилсеарчфолдер наследуется от mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ba76029b69d91be39c9d63ca755e8a4603aec0b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562607"
---
# <a name="mailsearchfolder-resource-type"></a>Тип ресурса Маилсеарчфолдер

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Маилсеарчфолдер — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска. Маилсеарчфолдер наследуется от [mailFolder](mailfolder.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип  | Описание |
|:---------------|:--------|:----------|
| [Создание папки поиска](../api/mailsearchfolder-post.md) | [Маилсеарчфолдер](mailsearchfolder.md) | Создайте папку поиска в почтовом ящике этого пользователя. |
| [Список папок поиска](../api/mailfolder-list-childfolders.md) | Коллекция [mailFolder](mailfolder.md) | ПереЧислите все папки в почтовом ящике этого пользователя, в том числе папки поиска. |
| [Получение папки поиска](../api/mailfolder-get.md) | [Маилсеарчфолдер](mailsearchfolder.md) | Получение указанной папки поиска. |
| [Обновление папки поиска](../api/mailsearchfolder-update.md) | [Маилсеарчфолдер](mailsearchfolder.md) | Обновление указанной папки поиска. |
| [Удаление папки поиска](../api/mailfolder-delete.md) | Нет | Удаление указанной папки поиска. |
| [ПереЧисление всех сообщений в папке поиска](../api/mailfolder-list-messages.md) | Коллекция объектов [message](message.md) | ПереЧисление всех сообщений в указанной папке поиска. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| Поддержка | Boolean | Указывает, является ли папка поиска редактируемой с помощью REST API. |
| Инклуденестедфолдерс | Boolean | Указывает, как должна проходить иерархия папок почтового ящика. `true`означает, что следует выполнить глубокий поиск, а `false` это означает, что вместо этого следует выполнить неглубокий Поиск. |
| Саурцефолдеридс | Коллекция String | Папки почтовых ящиков, которые должны быть mined. |
| Филтеркуери | String | Запрос OData для фильтрации сообщений. |

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
