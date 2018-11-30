---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: a849932d646be61f3cedec76ecdafdaca941baaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075587"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="ceda2-103">Тип ресурса office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="ceda2-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ceda2-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ceda2-104">Properties</span></span>

| <span data-ttu-id="ceda2-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ceda2-105">Property</span></span>                          | <span data-ttu-id="ceda2-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ceda2-106">Type</span></span>    | <span data-ttu-id="ceda2-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ceda2-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="ceda2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ceda2-108">reportRefreshDate</span></span>                 | <span data-ttu-id="ceda2-109">Date</span><span class="sxs-lookup"><span data-stu-id="ceda2-109">Date</span></span>    | <span data-ttu-id="ceda2-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="ceda2-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ceda2-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="ceda2-111">groupDisplayName</span></span>                  | <span data-ttu-id="ceda2-112">String</span><span class="sxs-lookup"><span data-stu-id="ceda2-112">String</span></span>  | <span data-ttu-id="ceda2-113">Отображаемое имя группы.</span><span class="sxs-lookup"><span data-stu-id="ceda2-113">The display name of the group.</span></span>           |
| <span data-ttu-id="ceda2-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ceda2-114">isDeleted</span></span>                         | <span data-ttu-id="ceda2-115">Логический</span><span class="sxs-lookup"><span data-stu-id="ceda2-115">Boolean</span></span> | <span data-ttu-id="ceda2-116">Был ли этот пользователь удаленного или программных удалены.</span><span class="sxs-lookup"><span data-stu-id="ceda2-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="ceda2-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ceda2-117">ownerPrincipalName</span></span>                | <span data-ttu-id="ceda2-118">String</span><span class="sxs-lookup"><span data-stu-id="ceda2-118">String</span></span>  | <span data-ttu-id="ceda2-119">Имя участника группы владельца.</span><span class="sxs-lookup"><span data-stu-id="ceda2-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="ceda2-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ceda2-120">lastActivityDate</span></span>                  | <span data-ttu-id="ceda2-121">Date</span><span class="sxs-lookup"><span data-stu-id="ceda2-121">Date</span></span>    | <span data-ttu-id="ceda2-122">Дата последнего действия для следующих сценариев: групповой полученных почтового ящика электронной почты; пользователю просматривать, редактировать, общих или синхронизирован файлы в библиотеке документов SharePoint. пользователь просматривает страницы SharePoint; пользователь учтена, чтение или оцененных сообщений в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="ceda2-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="ceda2-123">groupType</span><span class="sxs-lookup"><span data-stu-id="ceda2-123">groupType</span></span>                         | <span data-ttu-id="ceda2-124">String</span><span class="sxs-lookup"><span data-stu-id="ceda2-124">String</span></span>  | <span data-ttu-id="ceda2-125">Тип группы.</span><span class="sxs-lookup"><span data-stu-id="ceda2-125">The group type.</span></span> <span data-ttu-id="ceda2-126">Возможные значения: **Public** или **Private**.</span><span class="sxs-lookup"><span data-stu-id="ceda2-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="ceda2-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-127">memberCount</span></span>                       | <span data-ttu-id="ceda2-128">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-128">Int64</span></span>   | <span data-ttu-id="ceda2-129">Счетчик членов группы.</span><span class="sxs-lookup"><span data-stu-id="ceda2-129">The group member count.</span></span>                  |
| <span data-ttu-id="ceda2-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-130">externalMemberCount</span></span>               | <span data-ttu-id="ceda2-131">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-131">Int64</span></span>   | <span data-ttu-id="ceda2-132">Счетчик внешнего участника группы.</span><span class="sxs-lookup"><span data-stu-id="ceda2-132">The group external member count.</span></span>         |
| <span data-ttu-id="ceda2-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="ceda2-134">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-134">Int64</span></span>   | <span data-ttu-id="ceda2-135">Число электронной почты, полученных почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="ceda2-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="ceda2-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="ceda2-137">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-137">Int64</span></span>   | <span data-ttu-id="ceda2-138">Число активных файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ceda2-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="ceda2-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="ceda2-140">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-140">Int64</span></span>   | <span data-ttu-id="ceda2-141">Число сообщений, помещенных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="ceda2-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="ceda2-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="ceda2-143">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-143">Int64</span></span>   | <span data-ttu-id="ceda2-144">Количество сообщений, ознакомьтесь с разделом в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="ceda2-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="ceda2-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="ceda2-146">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-146">Int64</span></span>   | <span data-ttu-id="ceda2-147">Количество сообщений, оцененных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="ceda2-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="ceda2-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="ceda2-149">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-149">Int64</span></span>   | <span data-ttu-id="ceda2-150">Количество элементов в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="ceda2-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="ceda2-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ceda2-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="ceda2-152">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-152">Int64</span></span>   | <span data-ttu-id="ceda2-153">Хранения, используемый для почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="ceda2-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="ceda2-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="ceda2-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="ceda2-155">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-155">Int64</span></span>   | <span data-ttu-id="ceda2-156">Общее число файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ceda2-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="ceda2-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ceda2-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="ceda2-158">Int64</span><span class="sxs-lookup"><span data-stu-id="ceda2-158">Int64</span></span>   | <span data-ttu-id="ceda2-159">Хранилище, используемое сайта группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ceda2-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="ceda2-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ceda2-160">reportPeriod</span></span>                      | <span data-ttu-id="ceda2-161">String</span><span class="sxs-lookup"><span data-stu-id="ceda2-161">String</span></span>  | <span data-ttu-id="ceda2-162">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="ceda2-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ceda2-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ceda2-163">JSON representation</span></span>

<span data-ttu-id="ceda2-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ceda2-164">The following is a JSON representation of the resource.</span></span>

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
