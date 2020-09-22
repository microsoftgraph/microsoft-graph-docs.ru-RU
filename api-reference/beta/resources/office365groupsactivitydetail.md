---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: b7e22c522bf6cffeba6f09c350abaaabeda23b1b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092414"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="3cfa7-103">Тип ресурса office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="3cfa7-103">office365GroupsActivityDetail resource type</span></span>

<span data-ttu-id="3cfa7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cfa7-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3cfa7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cfa7-105">Properties</span></span>

| <span data-ttu-id="3cfa7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3cfa7-106">Property</span></span>                          | <span data-ttu-id="3cfa7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3cfa7-107">Type</span></span>    | <span data-ttu-id="3cfa7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3cfa7-108">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="3cfa7-109">groupId</span><span class="sxs-lookup"><span data-stu-id="3cfa7-109">groupId</span></span>                           | <span data-ttu-id="3cfa7-110">String</span><span class="sxs-lookup"><span data-stu-id="3cfa7-110">String</span></span>  | <span data-ttu-id="3cfa7-111">Идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-111">The group id.</span></span>          |
| <span data-ttu-id="3cfa7-112">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="3cfa7-112">reportRefreshDate</span></span>                 | <span data-ttu-id="3cfa7-113">Дата</span><span class="sxs-lookup"><span data-stu-id="3cfa7-113">Date</span></span>    | <span data-ttu-id="3cfa7-114">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-114">The latest date of the content.</span></span>          |
| <span data-ttu-id="3cfa7-115">граупдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="3cfa7-115">groupDisplayName</span></span>                  | <span data-ttu-id="3cfa7-116">Строка</span><span class="sxs-lookup"><span data-stu-id="3cfa7-116">String</span></span>  | <span data-ttu-id="3cfa7-117">Отображаемое имя группы.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-117">The display name of the group.</span></span>           |
| <span data-ttu-id="3cfa7-118">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3cfa7-118">isDeleted</span></span>                         | <span data-ttu-id="3cfa7-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cfa7-119">Boolean</span></span> | <span data-ttu-id="3cfa7-120">Указывает, был ли этот пользователь удален или обратимо удален.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-120">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="3cfa7-121">овнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="3cfa7-121">ownerPrincipalName</span></span>                | <span data-ttu-id="3cfa7-122">Строка</span><span class="sxs-lookup"><span data-stu-id="3cfa7-122">String</span></span>  | <span data-ttu-id="3cfa7-123">Имя участника владельца группы.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-123">The group owner principal name.</span></span>          |
| <span data-ttu-id="3cfa7-124">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="3cfa7-124">lastActivityDate</span></span>                  | <span data-ttu-id="3cfa7-125">Дата</span><span class="sxs-lookup"><span data-stu-id="3cfa7-125">Date</span></span>    | <span data-ttu-id="3cfa7-126">Дата последнего действия для следующих сценариев: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-126">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="3cfa7-127">groupType</span><span class="sxs-lookup"><span data-stu-id="3cfa7-127">groupType</span></span>                         | <span data-ttu-id="3cfa7-128">Строка</span><span class="sxs-lookup"><span data-stu-id="3cfa7-128">String</span></span>  | <span data-ttu-id="3cfa7-129">Тип группы.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-129">The group type.</span></span> <span data-ttu-id="3cfa7-130">Возможные значения: **Public** или **Private**.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-130">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="3cfa7-131">мемберкаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-131">memberCount</span></span>                       | <span data-ttu-id="3cfa7-132">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-132">Int64</span></span>   | <span data-ttu-id="3cfa7-133">Число участников группы.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-133">The group member count.</span></span>                  |
| <span data-ttu-id="3cfa7-134">екстерналмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-134">externalMemberCount</span></span>               | <span data-ttu-id="3cfa7-135">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-135">Int64</span></span>   | <span data-ttu-id="3cfa7-136">Количество внешних участников группы.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-136">The group external member count.</span></span>         |
| <span data-ttu-id="3cfa7-137">ексчанжерецеиведемаилкаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-137">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="3cfa7-138">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-138">Int64</span></span>   | <span data-ttu-id="3cfa7-139">Количество сообщений электронной почты, принимаемых группового почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-139">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="3cfa7-140">шарепоинтактивефилекаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-140">sharePointActiveFileCount</span></span>         | <span data-ttu-id="3cfa7-141">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-141">Int64</span></span>   | <span data-ttu-id="3cfa7-142">Количество активных файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-142">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="3cfa7-143">яммерпостедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-143">yammerPostedMessageCount</span></span>          | <span data-ttu-id="3cfa7-144">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-144">Int64</span></span>   | <span data-ttu-id="3cfa7-145">Количество сообщений, отправленных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-145">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="3cfa7-146">яммерреадмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-146">yammerReadMessageCount</span></span>            | <span data-ttu-id="3cfa7-147">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-147">Int64</span></span>   | <span data-ttu-id="3cfa7-148">Количество сообщений, прочитанных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-148">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="3cfa7-149">яммерликедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-149">yammerLikedMessageCount</span></span>           | <span data-ttu-id="3cfa7-150">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-150">Int64</span></span>   | <span data-ttu-id="3cfa7-151">Количество сообщений, которые понравилось в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-151">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="3cfa7-152">ексчанжемаилбокстоталитемкаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-152">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="3cfa7-153">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-153">Int64</span></span>   | <span data-ttu-id="3cfa7-154">Количество элементов в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-154">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="3cfa7-155">ексчанжемаилбокссторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="3cfa7-155">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="3cfa7-156">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-156">Int64</span></span>   | <span data-ttu-id="3cfa7-157">Хранилище, используемое для почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-157">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="3cfa7-158">шарепоинттоталфилекаунт</span><span class="sxs-lookup"><span data-stu-id="3cfa7-158">sharePointTotalFileCount</span></span>          | <span data-ttu-id="3cfa7-159">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-159">Int64</span></span>   | <span data-ttu-id="3cfa7-160">Общее количество файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-160">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="3cfa7-161">шарепоинтситесторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="3cfa7-161">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="3cfa7-162">Int64</span><span class="sxs-lookup"><span data-stu-id="3cfa7-162">Int64</span></span>   | <span data-ttu-id="3cfa7-163">Хранилище, используемое сайтом группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-163">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="3cfa7-164">репортпериод</span><span class="sxs-lookup"><span data-stu-id="3cfa7-164">reportPeriod</span></span>                      | <span data-ttu-id="3cfa7-165">Строка</span><span class="sxs-lookup"><span data-stu-id="3cfa7-165">String</span></span>  | <span data-ttu-id="3cfa7-166">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-166">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="3cfa7-167">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3cfa7-167">JSON representation</span></span>

<span data-ttu-id="3cfa7-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cfa7-168">The following is a JSON representation of the resource.</span></span>

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


