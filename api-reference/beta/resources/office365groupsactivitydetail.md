---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: fe2df5614525f27b294bed93be7f3f9cd8170b30
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981510"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="c0df9-103">Тип ресурса office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="c0df9-103">office365GroupsActivityDetail resource type</span></span>

<span data-ttu-id="c0df9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0df9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c0df9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0df9-105">Properties</span></span>

| <span data-ttu-id="c0df9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0df9-106">Property</span></span>                          | <span data-ttu-id="c0df9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c0df9-107">Type</span></span>    | <span data-ttu-id="c0df9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c0df9-108">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="c0df9-109">groupId</span><span class="sxs-lookup"><span data-stu-id="c0df9-109">groupId</span></span>                           | <span data-ttu-id="c0df9-110">String</span><span class="sxs-lookup"><span data-stu-id="c0df9-110">String</span></span>  | <span data-ttu-id="c0df9-111">ИД группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-111">The group id.</span></span>          |
| <span data-ttu-id="c0df9-112">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c0df9-112">reportRefreshDate</span></span>                 | <span data-ttu-id="c0df9-113">Дата</span><span class="sxs-lookup"><span data-stu-id="c0df9-113">Date</span></span>    | <span data-ttu-id="c0df9-114">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="c0df9-114">The latest date of the content.</span></span>          |
| <span data-ttu-id="c0df9-115">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="c0df9-115">groupDisplayName</span></span>                  | <span data-ttu-id="c0df9-116">String</span><span class="sxs-lookup"><span data-stu-id="c0df9-116">String</span></span>  | <span data-ttu-id="c0df9-117">Отображаемого имени группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-117">The display name of the group.</span></span>           |
| <span data-ttu-id="c0df9-118">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c0df9-118">isDeleted</span></span>                         | <span data-ttu-id="c0df9-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0df9-119">Boolean</span></span> | <span data-ttu-id="c0df9-120">Был ли этот пользователь удален или удален с помягким образом.</span><span class="sxs-lookup"><span data-stu-id="c0df9-120">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="c0df9-121">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c0df9-121">ownerPrincipalName</span></span>                | <span data-ttu-id="c0df9-122">String</span><span class="sxs-lookup"><span data-stu-id="c0df9-122">String</span></span>  | <span data-ttu-id="c0df9-123">Имя владельца группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-123">The group owner principal name.</span></span>          |
| <span data-ttu-id="c0df9-124">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c0df9-124">lastActivityDate</span></span>                  | <span data-ttu-id="c0df9-125">Дата</span><span class="sxs-lookup"><span data-stu-id="c0df9-125">Date</span></span>    | <span data-ttu-id="c0df9-126">Дата последнего действия для следующих сценариев: почтовый ящик группы получил сообщение электронной почты; просматриваются, редактируются, совместно или синхронизируются файлы в библиотеке документов SharePoint; просматривались пользователем страницы SharePoint; пользователи опубликовали, прочитали или понравились сообщения в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c0df9-126">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="c0df9-127">groupType</span><span class="sxs-lookup"><span data-stu-id="c0df9-127">groupType</span></span>                         | <span data-ttu-id="c0df9-128">String</span><span class="sxs-lookup"><span data-stu-id="c0df9-128">String</span></span>  | <span data-ttu-id="c0df9-129">Тип группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-129">The group type.</span></span> <span data-ttu-id="c0df9-130">Возможные значения: **Public или** **Private**.</span><span class="sxs-lookup"><span data-stu-id="c0df9-130">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="c0df9-131">memberCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-131">memberCount</span></span>                       | <span data-ttu-id="c0df9-132">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-132">Int64</span></span>   | <span data-ttu-id="c0df9-133">Количество членов группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-133">The group member count.</span></span>                  |
| <span data-ttu-id="c0df9-134">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-134">externalMemberCount</span></span>               | <span data-ttu-id="c0df9-135">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-135">Int64</span></span>   | <span data-ttu-id="c0df9-136">Количество внешних членов группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-136">The group external member count.</span></span>         |
| <span data-ttu-id="c0df9-137">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-137">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="c0df9-138">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-138">Int64</span></span>   | <span data-ttu-id="c0df9-139">Количество сообщений электронной почты, полученных почтовым ящиком группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-139">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="c0df9-140">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-140">sharePointActiveFileCount</span></span>         | <span data-ttu-id="c0df9-141">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-141">Int64</span></span>   | <span data-ttu-id="c0df9-142">Количество активных файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c0df9-142">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="c0df9-143">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-143">yammerPostedMessageCount</span></span>          | <span data-ttu-id="c0df9-144">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-144">Int64</span></span>   | <span data-ttu-id="c0df9-145">Количество сообщений, которые были опубликованы в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c0df9-145">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="c0df9-146">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-146">yammerReadMessageCount</span></span>            | <span data-ttu-id="c0df9-147">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-147">Int64</span></span>   | <span data-ttu-id="c0df9-148">Количество сообщений, прочитано в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c0df9-148">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="c0df9-149">yammerАedMessageCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-149">yammerLikedMessageCount</span></span>           | <span data-ttu-id="c0df9-150">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-150">Int64</span></span>   | <span data-ttu-id="c0df9-151">Количество сообщений, которые нравится в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c0df9-151">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="c0df9-152">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-152">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="c0df9-153">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-153">Int64</span></span>   | <span data-ttu-id="c0df9-154">Количество элементов в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-154">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="c0df9-155">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c0df9-155">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="c0df9-156">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-156">Int64</span></span>   | <span data-ttu-id="c0df9-157">Хранилище, используемого почтовым ящиком группы.</span><span class="sxs-lookup"><span data-stu-id="c0df9-157">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="c0df9-158">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="c0df9-158">sharePointTotalFileCount</span></span>          | <span data-ttu-id="c0df9-159">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-159">Int64</span></span>   | <span data-ttu-id="c0df9-160">Общее количество файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c0df9-160">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="c0df9-161">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c0df9-161">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="c0df9-162">Int64</span><span class="sxs-lookup"><span data-stu-id="c0df9-162">Int64</span></span>   | <span data-ttu-id="c0df9-163">Хранилище, используемого сайтом группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c0df9-163">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="c0df9-164">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c0df9-164">reportPeriod</span></span>                      | <span data-ttu-id="c0df9-165">String</span><span class="sxs-lookup"><span data-stu-id="c0df9-165">String</span></span>  | <span data-ttu-id="c0df9-166">Количество дней в отчете.</span><span class="sxs-lookup"><span data-stu-id="c0df9-166">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c0df9-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0df9-167">JSON representation</span></span>

<span data-ttu-id="c0df9-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0df9-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
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


