---
title: Настройка встроенных типов вкладок в Microsoft Teams
description: Создание или настройка вкладки Microsoft Teams с помощью API Microsoft Graph
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 888194fefef2e04f60ae802d5f8d710ba4388a97
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288933"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a><span data-ttu-id="c1669-103">Настройка встроенных типов вкладок в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c1669-103">Configuring the built-in tab types in Microsoft Teams</span></span>

<span data-ttu-id="c1669-104">Чтобы [создать](/graph/api/teamstab-add?view=graph-rest-beta) или [настроить](/graph/api/teamstab-update?view=graph-rest-beta) вкладку Microsoft Teams с помощью API Microsoft Graph, нужно знать значение `teamsAppId` приложения, и предоставить для этого типа приложения значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl`.</span><span class="sxs-lookup"><span data-stu-id="c1669-104">To [create](/graph/api/teamstab-add?view=graph-rest-beta) or [configure](/graph/api/teamstab-update?view=graph-rest-beta) a Microsoft Teams tab using Microsoft Graph APIs, you need to know the `teamsAppId` of the app, and the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` to provide for that kind of app.</span></span>
<span data-ttu-id="c1669-105">В этой статье объясняется, как получить эти значения для встроенных типов вкладок.</span><span class="sxs-lookup"><span data-stu-id="c1669-105">This article explains how to get those values for the built-in tab types.</span></span>

## <a name="custom-tabs"></a><span data-ttu-id="c1669-106">Настраиваемые вкладки</span><span class="sxs-lookup"><span data-stu-id="c1669-106">Custom tabs</span></span>

<span data-ttu-id="c1669-107">Чтобы использовать Microsoft Graph для настройки вкладки, связанной с [поставщиком вкладок](/microsoftteams/platform/concepts/tabs/tabs-overview), которого вы записали, определите значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl`, предоставляемые [интерфейсом конфигурации приложения для Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest), и передайте эти же значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl` в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c1669-107">To use Microsoft Graph to configure a tab associated with a [tab provider](/microsoftteams/platform/concepts/tabs/tabs-overview) that you wrote, identify the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` that the app's [configuration UI provides to Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest), and pass the same `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` values to Microsoft Graph.</span></span>

<span data-ttu-id="c1669-108">Объект `teamsAppId` аналогичен `id` в [схеме манифеста приложения для Microsoft Teams](/microsoftteams/platform/resources/schema/manifest-schema).</span><span class="sxs-lookup"><span data-stu-id="c1669-108">The `teamsAppId` is the same as the `id` in the [app manifest schema for Microsoft Teams](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>

## <a name="website-tabs"></a><span data-ttu-id="c1669-109">Вкладки веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="c1669-109">Website tabs</span></span>

<span data-ttu-id="c1669-110">Для вкладок веб-сайтов объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.web`.</span><span class="sxs-lookup"><span data-stu-id="c1669-110">For website tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.web`.</span></span> <span data-ttu-id="c1669-111">Ниже приведена конфигурация.</span><span class="sxs-lookup"><span data-stu-id="c1669-111">The following is the configuration.</span></span>

| <span data-ttu-id="c1669-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1669-112">Property</span></span>   | <span data-ttu-id="c1669-113">Тип</span><span class="sxs-lookup"><span data-stu-id="c1669-113">Type</span></span>        | <span data-ttu-id="c1669-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c1669-114">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="c1669-115">entityId</span><span class="sxs-lookup"><span data-stu-id="c1669-115">entityId</span></span>   | <span data-ttu-id="c1669-116">string</span><span class="sxs-lookup"><span data-stu-id="c1669-116">string</span></span>      | <span data-ttu-id="c1669-117">NULL</span><span class="sxs-lookup"><span data-stu-id="c1669-117">Null</span></span>                                                     |
| <span data-ttu-id="c1669-118">contentUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-118">contentUrl</span></span> | <span data-ttu-id="c1669-119">строка</span><span class="sxs-lookup"><span data-stu-id="c1669-119">string</span></span>      | <span data-ttu-id="c1669-120">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="c1669-120">URL of the website</span></span>                                       |
| <span data-ttu-id="c1669-121">removeUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-121">removeUrl</span></span>  | <span data-ttu-id="c1669-122">строка</span><span class="sxs-lookup"><span data-stu-id="c1669-122">string</span></span>      | <span data-ttu-id="c1669-123">NULL</span><span class="sxs-lookup"><span data-stu-id="c1669-123">Null</span></span>                                                     |
| <span data-ttu-id="c1669-124">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-124">websiteUrl</span></span> | <span data-ttu-id="c1669-125">строка</span><span class="sxs-lookup"><span data-stu-id="c1669-125">string</span></span>      | <span data-ttu-id="c1669-126">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="c1669-126">URL of the website</span></span>                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a><span data-ttu-id="c1669-127">Вкладки Word, Excel, PowerPoint и PDF</span><span class="sxs-lookup"><span data-stu-id="c1669-127">Word, Excel, PowerPoint, and PDF tabs</span></span>

<span data-ttu-id="c1669-128">В таблице ниже указаны `teamsAppId` для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="c1669-128">The following table lists the `teamsAppId` for each app.</span></span>

| <span data-ttu-id="c1669-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="c1669-129">App</span></span>   | <span data-ttu-id="c1669-130">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="c1669-130">teamsAppId</span></span> | <span data-ttu-id="c1669-131">Тип (расширение)</span><span class="sxs-lookup"><span data-stu-id="c1669-131">type (extension)</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="c1669-132">Word</span><span class="sxs-lookup"><span data-stu-id="c1669-132">Word</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| <span data-ttu-id="c1669-133">Excel</span><span class="sxs-lookup"><span data-stu-id="c1669-133">Excel</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| <span data-ttu-id="c1669-134">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="c1669-134">PowerPoint</span></span>  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| <span data-ttu-id="c1669-135">PDF</span><span class="sxs-lookup"><span data-stu-id="c1669-135">PDF</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

<span data-ttu-id="c1669-136">Ниже приведена конфигурация.</span><span class="sxs-lookup"><span data-stu-id="c1669-136">The following is the configuration.</span></span>

| <span data-ttu-id="c1669-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1669-137">Property</span></span>   | <span data-ttu-id="c1669-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c1669-138">Type</span></span>        | <span data-ttu-id="c1669-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c1669-139">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="c1669-140">entityId</span><span class="sxs-lookup"><span data-stu-id="c1669-140">entityId</span></span>   | <span data-ttu-id="c1669-141">string</span><span class="sxs-lookup"><span data-stu-id="c1669-141">string</span></span>      | <span data-ttu-id="c1669-142">Идентификатор sourceDoc для файла.</span><span class="sxs-lookup"><span data-stu-id="c1669-142">The sourceDoc ID of the file.</span></span> <span data-ttu-id="c1669-143">Вы найдете его, открыв файл в SharePoint и посмотрев на адресную строку — URL-адрес будет иметь предложение `sourcedoc=%7B{sourceDocId}%7D`.</span><span class="sxs-lookup"><span data-stu-id="c1669-143">You can find this by opening the file in SharePoint and looking at the address bar – the URL will have a `sourcedoc=%7B{sourceDocId}%7D` clause.</span></span> <span data-ttu-id="c1669-144">Вы также можете получить эти данные из webUrl адреса элемента диска SharePoint для документа.</span><span class="sxs-lookup"><span data-stu-id="c1669-144">You can also derive this from the webUrl of the SharePoint drive item for the document.</span></span> <span data-ttu-id="c1669-145">Дополнительные сведения см.[GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="c1669-145">For details, see [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="c1669-146">contentUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-146">contentUrl</span></span> | <span data-ttu-id="c1669-147">string</span><span class="sxs-lookup"><span data-stu-id="c1669-147">string</span></span>      | <span data-ttu-id="c1669-148">URL-адрес документ в формате `{folder-webUrl}/{item-name}`.</span><span class="sxs-lookup"><span data-stu-id="c1669-148">The URL of file in the format `{folder-webUrl}/{item-name}`.</span></span> <span data-ttu-id="c1669-149">{folder-webUrl} - это webUrl адрес папки SharePoint, содержащей файл, который можно найти путем открытия файла в SharePoint и просмотра адресной строки, либо с помощью свойства webUrl из [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="c1669-149">{folder-webUrl} is the webUrl of the SharePoint folder containing the file, which can be found by opening the file in SharePoint and looking at the address bar, or by using the webUrl property from [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> <span data-ttu-id="c1669-150">{item-name} соответствует имени файла (например, file.docx), которое является свойством `name` в [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="c1669-150">{item-name} is the file name (for example, file.docx), which is the `name` property in [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="c1669-151">removeUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-151">removeUrl</span></span>  | <span data-ttu-id="c1669-152">строка</span><span class="sxs-lookup"><span data-stu-id="c1669-152">string</span></span>      | <span data-ttu-id="c1669-153">NULL</span><span class="sxs-lookup"><span data-stu-id="c1669-153">Null</span></span>                                                     |
| <span data-ttu-id="c1669-154">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-154">websiteUrl</span></span> | <span data-ttu-id="c1669-155">string</span><span class="sxs-lookup"><span data-stu-id="c1669-155">string</span></span>      | <span data-ttu-id="c1669-156">Null</span><span class="sxs-lookup"><span data-stu-id="c1669-156">Null</span></span>                                       |

### <a name="example-create-a-configured-word-tab"></a><span data-ttu-id="c1669-157">Пример: создание настроенной вкладки Word</span><span class="sxs-lookup"><span data-stu-id="c1669-157">Example: Create a configured Word tab</span></span>

<span data-ttu-id="c1669-158">Приведенный ниже пример создает настроенную вкладку Word.</span><span class="sxs-lookup"><span data-stu-id="c1669-158">The following example creates a configured Word tab.</span></span>

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

## <a name="document-library-tabs"></a><span data-ttu-id="c1669-159">Вкладки библиотеки документов</span><span class="sxs-lookup"><span data-stu-id="c1669-159">Document library tabs</span></span>

<span data-ttu-id="c1669-160">Для вкладок библиотеки документов объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.files.sharepoint`.</span><span class="sxs-lookup"><span data-stu-id="c1669-160">For document library tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.files.sharepoint`.</span></span> <span data-ttu-id="c1669-161">Ниже приведена конфигурация.</span><span class="sxs-lookup"><span data-stu-id="c1669-161">The following is the configuration.</span></span>

| <span data-ttu-id="c1669-162">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1669-162">Property</span></span>   | <span data-ttu-id="c1669-163">Тип</span><span class="sxs-lookup"><span data-stu-id="c1669-163">Type</span></span>        | <span data-ttu-id="c1669-164">Описание</span><span class="sxs-lookup"><span data-stu-id="c1669-164">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="c1669-165">entityId</span><span class="sxs-lookup"><span data-stu-id="c1669-165">entityId</span></span>   | <span data-ttu-id="c1669-166">string</span><span class="sxs-lookup"><span data-stu-id="c1669-166">string</span></span>      | <span data-ttu-id="c1669-167">Пустая строка ("")</span><span class="sxs-lookup"><span data-stu-id="c1669-167">Empty string ("")</span></span>                                        |
| <span data-ttu-id="c1669-168">contentUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-168">contentUrl</span></span> | <span data-ttu-id="c1669-169">string</span><span class="sxs-lookup"><span data-stu-id="c1669-169">string</span></span>      | <span data-ttu-id="c1669-170">URL-адрес корневой папки библиотеки документов.</span><span class="sxs-lookup"><span data-stu-id="c1669-170">The URL of the root folder of the document library.</span></span> <span data-ttu-id="c1669-171">Этот URL-адрес можно найти, открыв папку SharePoint в браузере, скопировав URL-адрес и удалив "/Формс/аллитемс.аспкс" и все после этого.</span><span class="sxs-lookup"><span data-stu-id="c1669-171">You can find this URL by opening the SharePoint folder in your browser, copying the URL, and deleting "/Forms/AllItems.aspx" and everything after that.</span></span> |
| <span data-ttu-id="c1669-172">removeUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-172">removeUrl</span></span>  | <span data-ttu-id="c1669-173">строка</span><span class="sxs-lookup"><span data-stu-id="c1669-173">string</span></span>      | <span data-ttu-id="c1669-174">NULL</span><span class="sxs-lookup"><span data-stu-id="c1669-174">Null</span></span>                                                     |
| <span data-ttu-id="c1669-175">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="c1669-175">websiteUrl</span></span> | <span data-ttu-id="c1669-176">string</span><span class="sxs-lookup"><span data-stu-id="c1669-176">string</span></span>      | <span data-ttu-id="c1669-177">Null</span><span class="sxs-lookup"><span data-stu-id="c1669-177">Null</span></span>                                                     |

### <a name="example-create-a-configured-document-library-tab"></a><span data-ttu-id="c1669-178">Пример: создание настроенной вкладки библиотеки документов</span><span class="sxs-lookup"><span data-stu-id="c1669-178">Example: Create a configured document library tab</span></span>

<span data-ttu-id="c1669-179">Приведенный ниже пример создает настроенную вкладку Word.</span><span class="sxs-lookup"><span data-stu-id="c1669-179">The following example creates a configured Word tab.</span></span>

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

## <a name="wiki-tabs"></a><span data-ttu-id="c1669-180">Вкладки вики-сайта</span><span class="sxs-lookup"><span data-stu-id="c1669-180">Wiki tabs</span></span>

<span data-ttu-id="c1669-181">Для вкладок вики-сайта объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.wiki`.</span><span class="sxs-lookup"><span data-stu-id="c1669-181">For wiki tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.wiki`.</span></span>
<span data-ttu-id="c1669-182">Вкладки вики-сайта не поддерживают конфигурацию через Graph.</span><span class="sxs-lookup"><span data-stu-id="c1669-182">Wiki tabs do not support configuration through Graph.</span></span>
<span data-ttu-id="c1669-183">Однако обратите внимание, что практически отсутствуют параметры для конфигурации — в ненастроенной вкладке вики-сайта первому пользователю просто нужно выбрать **Настройка вкладки**, чтобы выполнить ее настройку.</span><span class="sxs-lookup"><span data-stu-id="c1669-183">Note, however, that there isn't much to configure -- in an un-configured wiki tab, the first user just needs to select **Set up tab** to configure it.</span></span>

## <a name="planner-tabs"></a><span data-ttu-id="c1669-184">Вкладки планировщика</span><span class="sxs-lookup"><span data-stu-id="c1669-184">Planner tabs</span></span>

<span data-ttu-id="c1669-185">Для вкладок планировщика объекту teamsAppId соответствует `com.microsoft.teamspace.tab.planner`.</span><span class="sxs-lookup"><span data-stu-id="c1669-185">For Planner tabs, the teamsAppId is `com.microsoft.teamspace.tab.planner`.</span></span> <span data-ttu-id="c1669-186">Конфигурация не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1669-186">Configuration is not supported.</span></span>

## <a name="microsoft-stream-tabs"></a><span data-ttu-id="c1669-187">Вкладки Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="c1669-187">Microsoft Stream tabs</span></span>

<span data-ttu-id="c1669-188">Для вкладок Microsoft Stream объекту `teamsAppId` соответствует `com.microsoftstream.embed.skypeteamstab`.</span><span class="sxs-lookup"><span data-stu-id="c1669-188">For Microsoft Stream tabs, the `teamsAppId` is `com.microsoftstream.embed.skypeteamstab`.</span></span> <span data-ttu-id="c1669-189">Конфигурация не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1669-189">Configuration is not supported.</span></span>

## <a name="microsoft-forms-tabs"></a><span data-ttu-id="c1669-190">Вкладки Microsoft Forms</span><span class="sxs-lookup"><span data-stu-id="c1669-190">Microsoft Forms tabs</span></span>

<span data-ttu-id="c1669-191">Для вкладок Microsoft Forms объекту `teamsAppId` соответствует `81fef3a6-72aa-4648-a763-de824aeafb7d`.</span><span class="sxs-lookup"><span data-stu-id="c1669-191">For Microsoft Forms tabs, the `teamsAppId` is `81fef3a6-72aa-4648-a763-de824aeafb7d`.</span></span>
<span data-ttu-id="c1669-192">Конфигурация не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1669-192">Configuration is not supported.</span></span>

## <a name="onenote-tabs"></a><span data-ttu-id="c1669-193">Вкладки OneNote</span><span class="sxs-lookup"><span data-stu-id="c1669-193">OneNote tabs</span></span>

<span data-ttu-id="c1669-194">Для вкладок OneNote объекту `teamsAppId` соответствует `0d820ecd-def2-4297-adad-78056cde7c78`.</span><span class="sxs-lookup"><span data-stu-id="c1669-194">For OneNote tabs, the `teamsAppId` is `0d820ecd-def2-4297-adad-78056cde7c78`.</span></span> <span data-ttu-id="c1669-195">Конфигурация не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1669-195">Configuration is not supported.</span></span>

## <a name="power-bi-tabs"></a><span data-ttu-id="c1669-196">Вкладки Power BI</span><span class="sxs-lookup"><span data-stu-id="c1669-196">Power BI tabs</span></span>

<span data-ttu-id="c1669-197">Для вкладок Power BI объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.powerbi`.</span><span class="sxs-lookup"><span data-stu-id="c1669-197">For Power BI tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.powerbi`.</span></span>
<span data-ttu-id="c1669-198">Конфигурация не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1669-198">Configuration is not supported.</span></span>

## <a name="sharepoint-page-and-list-tabs"></a><span data-ttu-id="c1669-199">Вкладки страниц и списков SharePoint</span><span class="sxs-lookup"><span data-stu-id="c1669-199">SharePoint page and list tabs</span></span>

<span data-ttu-id="c1669-200">Для вкладок страниц и списков SharePoint объекту `teamsAppId` соответствует `2a527703-1f6f-4559-a332-d8a7d288cd88`.</span><span class="sxs-lookup"><span data-stu-id="c1669-200">For SharePoint page and list tabs, the `teamsAppId` is `2a527703-1f6f-4559-a332-d8a7d288cd88`.</span></span>
<span data-ttu-id="c1669-201">Конфигурация не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1669-201">Configuration is not supported.</span></span>
<span data-ttu-id="c1669-202">Если вы хотите настроить вкладку, попробуйте использовать вкладку веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="c1669-202">If you want to configure the tab, consider using a Website tab.</span></span>