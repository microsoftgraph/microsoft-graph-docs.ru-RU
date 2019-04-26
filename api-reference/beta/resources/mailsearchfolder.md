---
title: Тип ресурса Маилсеарчфолдер
description: Маилсеарчфолдер — это виртуальная папка в почтовом ящике пользователя, содержащая все элементы электронной почты, удовлетворяющие указанным условиям поиска. Маилсеарчфолдер наследуется от mailFolder.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 15f334f2910c962c367242965bd2104c8f3edb79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342765"
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
| [ПереЧисление всех сообщений в папке поиска](../api/mailfolder-list-messages.md) | Коллекция [message](message.md) | ПереЧисление всех сообщений в указанной папке поиска. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| Поддержка | Логический | Указывает, является ли папка поиска редактируемой с помощью REST API. |
| Инклуденестедфолдерс | Логический | Указывает, как должна проходить иерархия папок почтового ящика. `true`означает, что следует выполнить глубокий поиск, а `false` это означает, что вместо этого следует выполнить неглубокий Поиск. |
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
  "suppressions": []
}
-->
