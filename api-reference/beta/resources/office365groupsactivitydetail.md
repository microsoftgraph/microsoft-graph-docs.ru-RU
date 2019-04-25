---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581452"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="57433-103">Тип ресурса office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="57433-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="57433-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="57433-104">Properties</span></span>

| <span data-ttu-id="57433-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="57433-105">Property</span></span>                          | <span data-ttu-id="57433-106">Тип</span><span class="sxs-lookup"><span data-stu-id="57433-106">Type</span></span>    | <span data-ttu-id="57433-107">Описание</span><span class="sxs-lookup"><span data-stu-id="57433-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="57433-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="57433-108">reportRefreshDate</span></span>                 | <span data-ttu-id="57433-109">Дата</span><span class="sxs-lookup"><span data-stu-id="57433-109">Date</span></span>    | <span data-ttu-id="57433-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="57433-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="57433-111">Граупдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="57433-111">groupDisplayName</span></span>                  | <span data-ttu-id="57433-112">String</span><span class="sxs-lookup"><span data-stu-id="57433-112">String</span></span>  | <span data-ttu-id="57433-113">Отображаемое имя группы.</span><span class="sxs-lookup"><span data-stu-id="57433-113">The display name of the group.</span></span>           |
| <span data-ttu-id="57433-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="57433-114">isDeleted</span></span>                         | <span data-ttu-id="57433-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="57433-115">Boolean</span></span> | <span data-ttu-id="57433-116">Указывает, был ли этот пользователь удален или обратимо удален.</span><span class="sxs-lookup"><span data-stu-id="57433-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="57433-117">ОвнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="57433-117">ownerPrincipalName</span></span>                | <span data-ttu-id="57433-118">String</span><span class="sxs-lookup"><span data-stu-id="57433-118">String</span></span>  | <span data-ttu-id="57433-119">Имя участника владельца группы.</span><span class="sxs-lookup"><span data-stu-id="57433-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="57433-120">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="57433-120">lastActivityDate</span></span>                  | <span data-ttu-id="57433-121">Дата</span><span class="sxs-lookup"><span data-stu-id="57433-121">Date</span></span>    | <span data-ttu-id="57433-122">Дата последнего действия для следующих сценариев: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="57433-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="57433-123">groupType</span><span class="sxs-lookup"><span data-stu-id="57433-123">groupType</span></span>                         | <span data-ttu-id="57433-124">String</span><span class="sxs-lookup"><span data-stu-id="57433-124">String</span></span>  | <span data-ttu-id="57433-125">Тип группы.</span><span class="sxs-lookup"><span data-stu-id="57433-125">The group type.</span></span> <span data-ttu-id="57433-126">Возможные значения: **Public** или **Private**.</span><span class="sxs-lookup"><span data-stu-id="57433-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="57433-127">Мемберкаунт</span><span class="sxs-lookup"><span data-stu-id="57433-127">memberCount</span></span>                       | <span data-ttu-id="57433-128">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-128">Int64</span></span>   | <span data-ttu-id="57433-129">Число участников группы.</span><span class="sxs-lookup"><span data-stu-id="57433-129">The group member count.</span></span>                  |
| <span data-ttu-id="57433-130">Екстерналмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="57433-130">externalMemberCount</span></span>               | <span data-ttu-id="57433-131">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-131">Int64</span></span>   | <span data-ttu-id="57433-132">Количество внешних участников группы.</span><span class="sxs-lookup"><span data-stu-id="57433-132">The group external member count.</span></span>         |
| <span data-ttu-id="57433-133">Ексчанжерецеиведемаилкаунт</span><span class="sxs-lookup"><span data-stu-id="57433-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="57433-134">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-134">Int64</span></span>   | <span data-ttu-id="57433-135">Количество сообщений электронной почты, принимаемых группового почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="57433-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="57433-136">Шарепоинтактивефилекаунт</span><span class="sxs-lookup"><span data-stu-id="57433-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="57433-137">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-137">Int64</span></span>   | <span data-ttu-id="57433-138">Количество активных файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57433-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="57433-139">Яммерпостедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="57433-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="57433-140">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-140">Int64</span></span>   | <span data-ttu-id="57433-141">Количество сообщений, отправленных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="57433-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="57433-142">Яммерреадмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="57433-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="57433-143">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-143">Int64</span></span>   | <span data-ttu-id="57433-144">Количество сообщений, прочитанных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="57433-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="57433-145">Яммерликедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="57433-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="57433-146">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-146">Int64</span></span>   | <span data-ttu-id="57433-147">Количество сообщений, которые понравилось в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="57433-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="57433-148">Ексчанжемаилбокстоталитемкаунт</span><span class="sxs-lookup"><span data-stu-id="57433-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="57433-149">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-149">Int64</span></span>   | <span data-ttu-id="57433-150">Количество элементов в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="57433-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="57433-151">Ексчанжемаилбокссторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="57433-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="57433-152">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-152">Int64</span></span>   | <span data-ttu-id="57433-153">Хранилище, используемое для почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="57433-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="57433-154">Шарепоинттоталфилекаунт</span><span class="sxs-lookup"><span data-stu-id="57433-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="57433-155">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-155">Int64</span></span>   | <span data-ttu-id="57433-156">Общее количество файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57433-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="57433-157">Шарепоинтситесторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="57433-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="57433-158">Int64</span><span class="sxs-lookup"><span data-stu-id="57433-158">Int64</span></span>   | <span data-ttu-id="57433-159">Хранилище, используемое сайтом группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57433-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="57433-160">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="57433-160">reportPeriod</span></span>                      | <span data-ttu-id="57433-161">String</span><span class="sxs-lookup"><span data-stu-id="57433-161">String</span></span>  | <span data-ttu-id="57433-162">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="57433-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="57433-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57433-163">JSON representation</span></span>

<span data-ttu-id="57433-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57433-164">The following is a JSON representation of the resource.</span></span>

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
