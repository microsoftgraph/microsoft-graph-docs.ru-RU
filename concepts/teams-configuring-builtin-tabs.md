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
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a><span data-ttu-id="6d660-103">Настройка встроенных типов вкладок в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6d660-103">Configuring the built-in tab types in Microsoft Teams</span></span>

<span data-ttu-id="6d660-104">Чтобы [создать](/graph/api/teamstab-add?view=graph-rest-beta) или [настроить](/graph/api/teamstab-update?view=graph-rest-beta) вкладку Microsoft Teams с помощью API Microsoft Graph, нужно знать значение `teamsAppId` приложения, и предоставить для этого типа приложения значения `entityId`, `contentUrl`, `removeUrl` и `websiteUrl`.</span><span class="sxs-lookup"><span data-stu-id="6d660-104">To [create](/graph/api/teamstab-add?view=graph-rest-beta) or [configure](/graph/api/teamstab-update?view=graph-rest-beta) a Microsoft Teams tab using Microsoft Graph APIs, you need to know the `teamsAppId` of the app, and the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` to provide for that kind of app.</span></span>
<span data-ttu-id="6d660-105">В этой статье объясняется, как получить эти значения для встроенных типов вкладок.</span><span class="sxs-lookup"><span data-stu-id="6d660-105">This article explains how to get those values for the built-in tab types.</span></span>

## <a name="website-tabs"></a><span data-ttu-id="6d660-106">Вкладки веб-сайтов</span><span class="sxs-lookup"><span data-stu-id="6d660-106">Website tabs</span></span>

<span data-ttu-id="6d660-107">Для вкладок веб-сайтов объекту `teamsAppId` соответствует `com.microsoft.teamspace.tab.web`.</span><span class="sxs-lookup"><span data-stu-id="6d660-107">For website tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.web`.</span></span> <span data-ttu-id="6d660-108">Ниже приведена конфигурация.</span><span class="sxs-lookup"><span data-stu-id="6d660-108">The following is the configuration.</span></span>

| <span data-ttu-id="6d660-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d660-109">Property</span></span>   | <span data-ttu-id="6d660-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6d660-110">Type</span></span>        | <span data-ttu-id="6d660-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6d660-111">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="6d660-112">entityId</span><span class="sxs-lookup"><span data-stu-id="6d660-112">entityId</span></span>   | <span data-ttu-id="6d660-113">string</span><span class="sxs-lookup"><span data-stu-id="6d660-113">string</span></span>      | <span data-ttu-id="6d660-114">Null</span><span class="sxs-lookup"><span data-stu-id="6d660-114">Null</span></span>                                                     |
| <span data-ttu-id="6d660-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="6d660-115">contentUrl</span></span> | <span data-ttu-id="6d660-116">строка</span><span class="sxs-lookup"><span data-stu-id="6d660-116">string</span></span>      | <span data-ttu-id="6d660-117">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="6d660-117">URL of the website</span></span>                                       |
| <span data-ttu-id="6d660-118">removeUrl</span><span class="sxs-lookup"><span data-stu-id="6d660-118">removeUrl</span></span>  | <span data-ttu-id="6d660-119">string</span><span class="sxs-lookup"><span data-stu-id="6d660-119">string</span></span>      | <span data-ttu-id="6d660-120">NULL</span><span class="sxs-lookup"><span data-stu-id="6d660-120">Null</span></span>                                                     |
| <span data-ttu-id="6d660-121">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="6d660-121">websiteUrl</span></span> | <span data-ttu-id="6d660-122">строка</span><span class="sxs-lookup"><span data-stu-id="6d660-122">string</span></span>      | <span data-ttu-id="6d660-123">URL-адрес веб-сайта</span><span class="sxs-lookup"><span data-stu-id="6d660-123">URL of the website</span></span>                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a><span data-ttu-id="6d660-124">Вкладки Word, Excel, PowerPoint и PDF</span><span class="sxs-lookup"><span data-stu-id="6d660-124">Word, Excel, PowerPoint, and PDF tabs</span></span>

<span data-ttu-id="6d660-125">В таблице ниже указаны `teamsAppId` для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="6d660-125">The following table lists the `teamsAppId` for each app.</span></span>

| <span data-ttu-id="6d660-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="6d660-126">App</span></span>   | <span data-ttu-id="6d660-127">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="6d660-127">teamsAppId</span></span> | <span data-ttu-id="6d660-128">Тип (расширение)</span><span class="sxs-lookup"><span data-stu-id="6d660-128">type (extension)</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="6d660-129">Word</span><span class="sxs-lookup"><span data-stu-id="6d660-129">Word</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| <span data-ttu-id="6d660-130">Excel</span><span class="sxs-lookup"><span data-stu-id="6d660-130">Excel</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| <span data-ttu-id="6d660-131">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="6d660-131">PowerPoint</span></span>  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| <span data-ttu-id="6d660-132">PDF</span><span class="sxs-lookup"><span data-stu-id="6d660-132">PDF</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

<span data-ttu-id="6d660-133">Ниже приведена конфигурация.</span><span class="sxs-lookup"><span data-stu-id="6d660-133">The following is the configuration.</span></span>

| <span data-ttu-id="6d660-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d660-134">Property</span></span>   | <span data-ttu-id="6d660-135">Тип</span><span class="sxs-lookup"><span data-stu-id="6d660-135">Type</span></span>        | <span data-ttu-id="6d660-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6d660-136">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="6d660-137">entityId</span><span class="sxs-lookup"><span data-stu-id="6d660-137">entityId</span></span>   | <span data-ttu-id="6d660-138">string</span><span class="sxs-lookup"><span data-stu-id="6d660-138">string</span></span>      | <span data-ttu-id="6d660-139">Идентификатор sourceDoc для файла.</span><span class="sxs-lookup"><span data-stu-id="6d660-139">The sourceDoc ID of the file.</span></span> <span data-ttu-id="6d660-140">Вы найдете его, открыв файл в SharePoint и посмотрев на адресную строку — URL-адрес будет иметь предложение `sourcedoc=%7B{sourceDocId}%7D`.</span><span class="sxs-lookup"><span data-stu-id="6d660-140">You can find this by opening the file in SharePoint and looking at the address bar – the URL will have a `sourcedoc=%7B{sourceDocId}%7D` clause.</span></span> <span data-ttu-id="6d660-141">Вы также можете получить эти данные из webUrl адреса элемента диска SharePoint для документа.</span><span class="sxs-lookup"><span data-stu-id="6d660-141">You can also derive this from the webUrl of the SharePoint drive item for the document.</span></span> <span data-ttu-id="6d660-142">Дополнительные сведения см.[GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="6d660-142">For details, see [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="6d660-143">contentUrl</span><span class="sxs-lookup"><span data-stu-id="6d660-143">contentUrl</span></span> | <span data-ttu-id="6d660-144">string</span><span class="sxs-lookup"><span data-stu-id="6d660-144">string</span></span>      | <span data-ttu-id="6d660-145">URL-адрес документ в формате `{folder-webUrl}/{item-name}`.</span><span class="sxs-lookup"><span data-stu-id="6d660-145">The URL of file in the format `{folder-webUrl}/{item-name}`.</span></span> <span data-ttu-id="6d660-146">{folder-webUrl} - это webUrl адрес папки SharePoint, содержащей файл, который можно найти путем открытия файла в SharePoint и просмотра адресной строки, либо с помощью свойства webUrl из [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="6d660-146">{folder-webUrl} is the webUrl of the SharePoint folder containing the file, which can be found by opening the file in SharePoint and looking at the address bar, or by using the webUrl property from [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> <span data-ttu-id="6d660-147">{item-name} соответствует имени файла (например, file.docx), которое является свойством `name` в [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="6d660-147">{item-name} is the file name (for example, file.docx), which is the `name` property in [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="6d660-148">removeUrl</span><span class="sxs-lookup"><span data-stu-id="6d660-148">removeUrl</span></span>  | <span data-ttu-id="6d660-149">string</span><span class="sxs-lookup"><span data-stu-id="6d660-149">string</span></span>      | <span data-ttu-id="6d660-150">NULL</span><span class="sxs-lookup"><span data-stu-id="6d660-150">Null</span></span>                                                     |
| <span data-ttu-id="6d660-151">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="6d660-151">websiteUrl</span></span> | <span data-ttu-id="6d660-152">string</span><span class="sxs-lookup"><span data-stu-id="6d660-152">string</span></span>      | <span data-ttu-id="6d660-153">Null</span><span class="sxs-lookup"><span data-stu-id="6d660-153">Null</span></span>                                       |

### <a name="example-create-a-configured-word-tab"></a><span data-ttu-id="6d660-154">Пример: создание настроенной вкладки Word</span><span class="sxs-lookup"><span data-stu-id="6d660-154">Example: Create a configured Word tab</span></span>

<span data-ttu-id="6d660-155">Приведенный ниже пример создает настроенную вкладку Word.</span><span class="sxs-lookup"><span data-stu-id="6d660-155">The following example creates a configured Word tab.</span></span>

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
