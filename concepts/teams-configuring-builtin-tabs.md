---
title: Настройка встроенных типов вкладок в Microsoft Teams
description: Создание или настройка вкладки Microsoft Teams с помощью API Microsoft Graph
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2940edf1cef2adc6c240fe8dd737d91f434c27e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574598"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>Настройка встроенных типов вкладок в Microsoft Teams

Чтобы [создать](/graph/api/teamstab-add?view=graph-rest-beta) или [настроить](/graph/api/teamstab-update?view=graph-rest-beta) вкладку Microsoft Teams с помощью API Microsoft Graph, нужно знать значение `teamsAppId` приложения, и предоставить для этого типа приложения значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl`.
В этой статье объясняется, как получить эти значения для встроенных типов вкладок.

## <a name="custom-tabs"></a>Настраиваемые вкладки

Чтобы использовать Microsoft Graph для настройки вкладки, связанной с [поставщиком вкладок](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview), которого вы записали, определите значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl`, предоставляемые [интерфейсом конфигурации приложения для Microsoft Teams](https://docs.microsoft.com/en-us/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest), и передайте эти же значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl` в Microsoft Graph.

Объект `teamsAppId` аналогичен `id` в [схеме манифеста приложения для Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/schema/manifest-schema).

## <a name="website-tabs"></a>Вкладки веб-сайтов

Для вкладок веб-сайтов объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.web`. Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | URL-адрес веб-сайта                                       |
| removeUrl  | string      | NULL                                                     |
| websiteUrl | string      | URL-адрес веб-сайта                                       |

## <a name="planner-tabs"></a>Вкладки планировщика

Для вкладок планировщика объекту teamsAppId соответствует `com.microsoft.teamspace.tab.planner`. Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Идентификатор плана (идентификатор для применения с действием GET /planner/plans/{id}).                                              |
| contentUrl | string      | `https://tasks.office.com/{tenantName}/Home/PlannerFrame?page=7&planId={planId}`, где {tenantName} — это имя клиента (например, example.onmicrosoft.com), а {planId} совпадает с идентификатором сущности.  |
| removeUrl  | string      | Совпадает со значением contentUrl.    |
| websiteUrl | string      | Совпадает со значением contentUrl.   |

Чтобы создать новый план для отображения на вкладке планировщика, см. статью [Создание объекта plannerPlan](/graph/api/planner-post-plans?view=graph-rest-beta).

## <a name="microsoft-stream-tabs"></a>Вкладки Microsoft Stream

Для вкладок Microsoft Stream объекту `teamsAppId` соответствует `com.microsoftstream.embed.skypeteamstab`. Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | `https://web.microsoftstream.com/embed/video/{id}?autoplay=false&showinfo=true&app=microsoftteams&l={locale}`, где {id} — это идентификатор видеопотока. Чтобы найти {id} потока, откройте его в браузере и взгляните на URL-адрес — он будет представлен в форме `https://{domain}.microsoftstream.com/video/{id}`.  |
| removeUrl  | string      | NULL                                                     |
| websiteUrl | string      | `https://web.microsoftstream.com/video/{id}`, где {id} — это идентификатор видеопотока.    |

## <a name="microsoft-forms-tabs"></a>Вкладки Microsoft Forms

Для вкладок Microsoft Forms объекту `teamsAppId` соответствует `81fef3a6-72aa-4648-a763-de824aeafb7d`.
Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Идентификатор формы.  Определите это значение, перейдите к форме на веб-сайте Forms и найдите URL-адрес формы `https://forms.office.com/Pages/DesignPage.aspx#FormId={formId}`.      |
| contentUrl | string      | `https://forms.office.com/Pages/TeamsDesignPage.aspx?Host=Teams&lang={locale}&groupId={groupId}&tid={tid}&teamsTheme={theme}&upn={upn}&fragment=FormId%3D{formId}`, где {formId} совпадает с идентификатором сущности, а {locale}, {groupId}, {tid}, {upn} являются литералами.   |
| removeUrl  | string      | NULL                                                     |
| websiteUrl | строка      |  `https://forms.office.com`    |

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
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/com.microsoft.teamspace.tab.file.staticviewer.word",
  "configuration": {
     "entityId": "115A90F4-AC9C-4F79-9837-36D1EFB3BE08",
     "contentUrl": "https://m365x165177.sharepoint.com/sites/4NewCloneWithClonableParts/Shared%20Documents/General/Employee Handbook.docx",
     "removeUrl": null,
     "websiteUrl": null
  }
}
```

## <a name="wiki-tabs"></a>Вкладки вики-сайта

Для вкладок вики-сайта объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.wiki`.
Вкладки вики-сайта не поддерживают конфигурацию через Graph.
Однако обратите внимание, что практически отсутствуют параметры для конфигурации — в ненастроенной вкладке вики-сайта первому пользователю просто нужно выбрать **Настройка вкладки**, чтобы выполнить ее настройку.

## <a name="document-library-tabs"></a>Вкладки библиотеки документов

Для вкладок библиотеки документов объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.files.sharepoint`. Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Пустая строка ("")                                        |
| contentUrl | string      | URL-адрес корневой папки библиотеки документов. Этот URL-адрес можно найти, открыв папку SharePoint в браузере, скопировав URL-адрес и удалив "/Формс/аллитемс.аспкс" и все после этого. |
| removeUrl  | string      | NULL                                                     |
| websiteUrl | string      | Null                                                     |

### <a name="example-create-a-configured-document-library-tab"></a>Пример: создание настроенной вкладки библиотеки документов

Приведенный ниже пример создает настроенную вкладку Word.

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

## <a name="onenote-tabs"></a>Вкладки OneNote

Для вкладок OneNote объекту `teamsAppId` соответствует `0d820ecd-def2-4297-adad-78056cde7c78`. Ниже приведена конфигурация.

| Свойство   | Тип        | Описание                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | `{randomGuid}_{notebookId}`, где {randomGuid} — это созданный вами идентификатор GUID.                                      |
| contentUrl | string      | URL-адрес формы `https://www.onenote.com/teams/TabContent?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`, где `{sectionsUrl}`, `{notebookId}` и `{oneNoteWebUrl}` можно найти в [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta). Символы косой черты необходимо пропустить. {locale} и {tid} являются литералами. |
| removeUrl  | string      | URL-адрес формы `https://www.onenote.com/teams/TabRemove?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`, где `{sectionsUrl}`, `{notebookId}` и `{oneNoteWebUrl}` можно найти в [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta). Символы косой черты необходимо пропустить. {locale} и {tid} являются литералами. |
| websiteUrl | строка      | URL-адрес формы `https://www.onenote.com/teams/TabRedirect?redirectUrl={oneNoteWebUrl}`, где `oneNoteWebUrl` можно найти в [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) |

## <a name="power-bi-tabs"></a>Вкладки Power BI

Для вкладок Power BI объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.powerbi`.
Конфигурация не поддерживается.

## <a name="sharepoint-page-and-list-tabs"></a>Вкладки страниц и списков SharePoint

Для вкладок страниц и списков SharePoint объекту `teamsAppId` соответствует `2a527703-1f6f-4559-a332-d8a7d288cd88`.
Конфигурация не поддерживается.
Если вы хотите настроить вкладку, попробуйте использовать вкладку веб-сайта.
