---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575120"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="7e099-103">Тип ресурса office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="7e099-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7e099-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e099-104">Properties</span></span>

| <span data-ttu-id="7e099-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e099-105">Property</span></span>                          | <span data-ttu-id="7e099-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7e099-106">Type</span></span>    | <span data-ttu-id="7e099-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7e099-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="7e099-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7e099-108">reportRefreshDate</span></span>                 | <span data-ttu-id="7e099-109">Date</span><span class="sxs-lookup"><span data-stu-id="7e099-109">Date</span></span>    | <span data-ttu-id="7e099-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="7e099-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="7e099-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="7e099-111">groupDisplayName</span></span>                  | <span data-ttu-id="7e099-112">Строка</span><span class="sxs-lookup"><span data-stu-id="7e099-112">String</span></span>  | <span data-ttu-id="7e099-113">Отображаемое имя группы.</span><span class="sxs-lookup"><span data-stu-id="7e099-113">The display name of the group.</span></span>           |
| <span data-ttu-id="7e099-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7e099-114">isDeleted</span></span>                         | <span data-ttu-id="7e099-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e099-115">Boolean</span></span> | <span data-ttu-id="7e099-116">Был ли этот пользователь удаленного или программных удалены.</span><span class="sxs-lookup"><span data-stu-id="7e099-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="7e099-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7e099-117">ownerPrincipalName</span></span>                | <span data-ttu-id="7e099-118">Строка</span><span class="sxs-lookup"><span data-stu-id="7e099-118">String</span></span>  | <span data-ttu-id="7e099-119">Имя участника группы владельца.</span><span class="sxs-lookup"><span data-stu-id="7e099-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="7e099-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7e099-120">lastActivityDate</span></span>                  | <span data-ttu-id="7e099-121">Date</span><span class="sxs-lookup"><span data-stu-id="7e099-121">Date</span></span>    | <span data-ttu-id="7e099-122">Дата последнего действия для следующих сценариев: групповой полученных почтового ящика электронной почты; пользователю просматривать, редактировать, общих или синхронизирован файлы в библиотеке документов SharePoint. пользователь просматривает страницы SharePoint; пользователь учтена, чтение или оцененных сообщений в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="7e099-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="7e099-123">groupType</span><span class="sxs-lookup"><span data-stu-id="7e099-123">groupType</span></span>                         | <span data-ttu-id="7e099-124">Строка</span><span class="sxs-lookup"><span data-stu-id="7e099-124">String</span></span>  | <span data-ttu-id="7e099-125">Тип группы.</span><span class="sxs-lookup"><span data-stu-id="7e099-125">The group type.</span></span> <span data-ttu-id="7e099-126">Возможные значения: **Public** или **Private**.</span><span class="sxs-lookup"><span data-stu-id="7e099-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="7e099-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="7e099-127">memberCount</span></span>                       | <span data-ttu-id="7e099-128">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-128">Int64</span></span>   | <span data-ttu-id="7e099-129">Счетчик членов группы.</span><span class="sxs-lookup"><span data-stu-id="7e099-129">The group member count.</span></span>                  |
| <span data-ttu-id="7e099-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="7e099-130">externalMemberCount</span></span>               | <span data-ttu-id="7e099-131">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-131">Int64</span></span>   | <span data-ttu-id="7e099-132">Счетчик внешнего участника группы.</span><span class="sxs-lookup"><span data-stu-id="7e099-132">The group external member count.</span></span>         |
| <span data-ttu-id="7e099-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="7e099-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="7e099-134">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-134">Int64</span></span>   | <span data-ttu-id="7e099-135">Число электронной почты, полученных почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="7e099-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="7e099-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="7e099-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="7e099-137">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-137">Int64</span></span>   | <span data-ttu-id="7e099-138">Число активных файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7e099-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="7e099-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="7e099-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="7e099-140">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-140">Int64</span></span>   | <span data-ttu-id="7e099-141">Число сообщений, помещенных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="7e099-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="7e099-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="7e099-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="7e099-143">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-143">Int64</span></span>   | <span data-ttu-id="7e099-144">Количество сообщений, ознакомьтесь с разделом в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="7e099-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="7e099-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="7e099-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="7e099-146">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-146">Int64</span></span>   | <span data-ttu-id="7e099-147">Количество сообщений, оцененных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="7e099-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="7e099-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="7e099-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="7e099-149">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-149">Int64</span></span>   | <span data-ttu-id="7e099-150">Количество элементов в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="7e099-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="7e099-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="7e099-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="7e099-152">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-152">Int64</span></span>   | <span data-ttu-id="7e099-153">Хранения, используемый для почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="7e099-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="7e099-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="7e099-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="7e099-155">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-155">Int64</span></span>   | <span data-ttu-id="7e099-156">Общее число файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7e099-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="7e099-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="7e099-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="7e099-158">Int64</span><span class="sxs-lookup"><span data-stu-id="7e099-158">Int64</span></span>   | <span data-ttu-id="7e099-159">Хранилище, используемое сайта группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7e099-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="7e099-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7e099-160">reportPeriod</span></span>                      | <span data-ttu-id="7e099-161">Строка</span><span class="sxs-lookup"><span data-stu-id="7e099-161">String</span></span>  | <span data-ttu-id="7e099-162">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="7e099-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="7e099-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e099-163">JSON representation</span></span>

<span data-ttu-id="7e099-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e099-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```
