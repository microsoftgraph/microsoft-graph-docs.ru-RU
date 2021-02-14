---
title: Настройка встроенных типов вкладок в Microsoft Teams
description: Создание или настройка вкладки Microsoft Teams с помощью API Microsoft Graph
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 13f0719a63cc604a8ffb9b77540e346837f1a031
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239445"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>Настройка встроенных типов вкладок в Microsoft Teams

Чтобы [создать](/graph/api/channel-post-tabs?view=graph-rest-1.0) или [настроить](/graph/api/channel-patch-tabs?view=graph-rest-1.0) вкладку Microsoft Teams с помощью API Microsoft Graph, нужно знать значение `teamsAppId` приложения, и предоставить для этого типа приложения значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl`.
В этой статье объясняется, как получить эти значения для встроенных типов вкладок.

## <a name="custom-tabs"></a>Настраиваемые вкладки

Чтобы использовать Microsoft Graph для настройки вкладки, связанной с [поставщиком вкладок](/microsoftteams/platform/concepts/tabs/tabs-overview), которого вы записали, определите значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl`, предоставляемые [интерфейсом конфигурации приложения для Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest), и передайте эти же значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl` в Microsoft Graph.

Объект `teamsAppId` аналогичен `id` в [схеме манифеста приложения для Microsoft Teams](/microsoftteams/platform/resources/schema/manifest-schema).

## <a name="website-tabs"></a>Вкладки веб-сайтов

Для вкладок веб-сайтов объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.web`. Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | NULL                                                     |
| contentUrl | строка      | URL-адрес веб-сайта                                       |
| removeUrl  | строка      | NULL                                                     |
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
| removeUrl  | строка      | NULL                                                     |
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

## <a name="document-library-tabs"></a>Вкладки библиотеки документов

Для вкладок библиотеки документов объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.files.sharepoint`. Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Пустая строка ("")                                        |
| contentUrl | string      | URL-адрес корневой папки библиотеки документов. Этот URL-адрес можно найти, открыв папку SharePoint в браузере, скопируйте URL-адрес и удалите "/Forms/AllItems.aspx" и все после этого. |
| removeUrl  | строка      | NULL                                                     |
| websiteUrl | string      | Null                                                     |

### <a name="example-create-a-configured-document-library-tab"></a>Пример: создание настроенной вкладки библиотеки документов

В следующем примере создается настроенная вкладка библиотеки документов.

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
    "displayName": "Document%20Library1",
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.files.sharepoint",
    "configuration": {
        "entityId": "",
        "contentUrl": "https://microsoft.sharepoint.com/teams/WWWtest/Shared%20Documents",
        "removeUrl": null,
        "websiteUrl": null
    }
}
```

## <a name="wiki-tabs"></a>Вкладки вики-сайта

Для вкладок вики-сайта объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.wiki`.
Вики-вкладки не поддерживают настройку с помощью Microsoft Graph.
Обратите внимание, что настраивать не так много— на ненастроеной вкладке вики-сайта первый пользователь должен выбрать вкладку "Настройка", чтобы настроить ее. 

## <a name="planner-tabs"></a>Вкладки планировщика

Для вкладок Планировщика это `teamsAppId` `com.microsoft.teamspace.tab.planner` . Конфигурация не поддерживается.

## <a name="microsoft-stream-tabs"></a>Вкладки Microsoft Stream

Для вкладок Microsoft Stream объекту `teamsAppId` соответствует `com.microsoftstream.embed.skypeteamstab`. Конфигурация не поддерживается.

## <a name="microsoft-forms-tabs"></a>Вкладки Microsoft Forms

Для вкладок Microsoft Forms объекту `teamsAppId` соответствует `81fef3a6-72aa-4648-a763-de824aeafb7d`.
Конфигурация не поддерживается.

## <a name="onenote-tabs"></a>Вкладки OneNote

Для вкладок OneNote объекту `teamsAppId` соответствует `0d820ecd-def2-4297-adad-78056cde7c78`. Конфигурация не поддерживается.

## <a name="power-bi-tabs"></a>Вкладки Power BI

Для вкладок Power BI объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.powerbi`.
Конфигурация не поддерживается.

## <a name="sharepoint-page-and-list-tabs"></a>Вкладки страниц и списков SharePoint

Для вкладок страниц и списков SharePoint объекту `teamsAppId` соответствует `2a527703-1f6f-4559-a332-d8a7d288cd88`.
Конфигурация не поддерживается.
Если вы хотите настроить вкладку, попробуйте использовать вкладку веб-сайта.
