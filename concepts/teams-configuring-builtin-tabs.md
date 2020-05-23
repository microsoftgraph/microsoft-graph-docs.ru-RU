---
title: Настройка встроенных типов вкладок в Microsoft Teams
description: Создание или настройка вкладки Microsoft Teams с помощью API Microsoft Graph
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ffe2799f557b12dd72fa72e6bf8b20f72f507647
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345991"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>Настройка встроенных типов вкладок в Microsoft Teams

Чтобы [создать](/graph/api/teamstab-add?view=graph-rest-beta) или [настроить](/graph/api/teamstab-update?view=graph-rest-beta) вкладку Microsoft Teams с помощью API Microsoft Graph, нужно знать значение `teamsAppId` приложения, и предоставить для этого типа приложения значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl`.
В этой статье объясняется, как получить эти значения для встроенных типов вкладок.

## <a name="website-tabs"></a>Вкладки веб-сайтов

Для вкладок веб-сайтов объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.web`. Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | строка      | URL-адрес веб-сайта                                       |
| removeUrl  | string      | NULL                                                     |
| websiteUrl | строка      | URL-адрес веб-сайта                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Вкладки Word, Excel, PowerPoint и PDF

В таблице ниже указаны `teamsAppId` для каждого приложения.

| Приложение   | teamsAppId | Тип (расширение)                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Идентификатор sourceDoc для файла. Вы найдете его, открыв файл в SharePoint и посмотрев на адресную строку — URL-адрес будет иметь предложение `sourcedoc=%7B{sourceDocId}%7D`. Вы также можете получить эти данные из webUrl адреса элемента диска SharePoint для документа. Дополнительные сведения см.[GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta). |
| contentUrl | string      | URL-адрес документ в формате `{folder-webUrl}/{item-name}`. {folder-webUrl} - это webUrl адрес папки SharePoint, содержащей файл, который можно найти путем открытия файла в SharePoint и просмотра адресной строки, либо с помощью свойства webUrl из [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta). {item-name} соответствует имени файла (например, file.docx), которое является свойством `name` в [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta). |
| removeUrl  | string      | NULL                                                     |
| websiteUrl | string      | Null                                       |

### <a name="example-create-a-configured-word-tab"></a>Пример: создание настроенной вкладки Word

Приведенный ниже пример создает настроенную вкладку Word.

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
  "displayName": "word",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.file.staticviewer.word",
  "configuration": {
     "entityId": "115A90F4-AC9C-4F79-9837-36D1EFB3BE08",
     "contentUrl": "https://m365x165177.sharepoint.com/sites/4NewCloneWithClonableParts/Shared%20Documents/General/Employee Handbook.docx",
     "removeUrl": null,
     "websiteUrl": null
  }
}
```
