---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: dfc45c4973194d26c1830f8c36d3bf3b407d2e3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009505"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="79d30-103">Тип ресурса office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="79d30-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="79d30-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="79d30-104">Properties</span></span>

| <span data-ttu-id="79d30-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="79d30-105">Property</span></span>                          | <span data-ttu-id="79d30-106">Тип</span><span class="sxs-lookup"><span data-stu-id="79d30-106">Type</span></span>    | <span data-ttu-id="79d30-107">Описание</span><span class="sxs-lookup"><span data-stu-id="79d30-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="79d30-108">groupId</span><span class="sxs-lookup"><span data-stu-id="79d30-108">groupId</span></span>                           | <span data-ttu-id="79d30-109">String</span><span class="sxs-lookup"><span data-stu-id="79d30-109">String</span></span>  | <span data-ttu-id="79d30-110">Идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="79d30-110">The group id.</span></span>          |
| <span data-ttu-id="79d30-111">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="79d30-111">reportRefreshDate</span></span>                 | <span data-ttu-id="79d30-112">Дата</span><span class="sxs-lookup"><span data-stu-id="79d30-112">Date</span></span>    | <span data-ttu-id="79d30-113">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="79d30-113">The latest date of the content.</span></span>          |
| <span data-ttu-id="79d30-114">Граупдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="79d30-114">groupDisplayName</span></span>                  | <span data-ttu-id="79d30-115">String</span><span class="sxs-lookup"><span data-stu-id="79d30-115">String</span></span>  | <span data-ttu-id="79d30-116">Отображаемое имя группы.</span><span class="sxs-lookup"><span data-stu-id="79d30-116">The display name of the group.</span></span>           |
| <span data-ttu-id="79d30-117">isDeleted</span><span class="sxs-lookup"><span data-stu-id="79d30-117">isDeleted</span></span>                         | <span data-ttu-id="79d30-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="79d30-118">Boolean</span></span> | <span data-ttu-id="79d30-119">Указывает, был ли этот пользователь удален или обратимо удален.</span><span class="sxs-lookup"><span data-stu-id="79d30-119">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="79d30-120">ОвнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="79d30-120">ownerPrincipalName</span></span>                | <span data-ttu-id="79d30-121">String</span><span class="sxs-lookup"><span data-stu-id="79d30-121">String</span></span>  | <span data-ttu-id="79d30-122">Имя участника владельца группы.</span><span class="sxs-lookup"><span data-stu-id="79d30-122">The group owner principal name.</span></span>          |
| <span data-ttu-id="79d30-123">Ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="79d30-123">lastActivityDate</span></span>                  | <span data-ttu-id="79d30-124">Дата</span><span class="sxs-lookup"><span data-stu-id="79d30-124">Date</span></span>    | <span data-ttu-id="79d30-125">Дата последнего действия для следующих сценариев: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="79d30-125">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="79d30-126">groupType</span><span class="sxs-lookup"><span data-stu-id="79d30-126">groupType</span></span>                         | <span data-ttu-id="79d30-127">String</span><span class="sxs-lookup"><span data-stu-id="79d30-127">String</span></span>  | <span data-ttu-id="79d30-128">Тип группы.</span><span class="sxs-lookup"><span data-stu-id="79d30-128">The group type.</span></span> <span data-ttu-id="79d30-129">Возможные значения: **Public** или **Private**.</span><span class="sxs-lookup"><span data-stu-id="79d30-129">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="79d30-130">Мемберкаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-130">memberCount</span></span>                       | <span data-ttu-id="79d30-131">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-131">Int64</span></span>   | <span data-ttu-id="79d30-132">Число участников группы.</span><span class="sxs-lookup"><span data-stu-id="79d30-132">The group member count.</span></span>                  |
| <span data-ttu-id="79d30-133">Екстерналмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-133">externalMemberCount</span></span>               | <span data-ttu-id="79d30-134">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-134">Int64</span></span>   | <span data-ttu-id="79d30-135">Количество внешних участников группы.</span><span class="sxs-lookup"><span data-stu-id="79d30-135">The group external member count.</span></span>         |
| <span data-ttu-id="79d30-136">Ексчанжерецеиведемаилкаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-136">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="79d30-137">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-137">Int64</span></span>   | <span data-ttu-id="79d30-138">Количество сообщений электронной почты, принимаемых группового почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="79d30-138">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="79d30-139">Шарепоинтактивефилекаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-139">sharePointActiveFileCount</span></span>         | <span data-ttu-id="79d30-140">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-140">Int64</span></span>   | <span data-ttu-id="79d30-141">Количество активных файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="79d30-141">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="79d30-142">Яммерпостедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-142">yammerPostedMessageCount</span></span>          | <span data-ttu-id="79d30-143">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-143">Int64</span></span>   | <span data-ttu-id="79d30-144">Количество сообщений, отправленных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="79d30-144">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="79d30-145">Яммерреадмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-145">yammerReadMessageCount</span></span>            | <span data-ttu-id="79d30-146">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-146">Int64</span></span>   | <span data-ttu-id="79d30-147">Количество сообщений, прочитанных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="79d30-147">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="79d30-148">Яммерликедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-148">yammerLikedMessageCount</span></span>           | <span data-ttu-id="79d30-149">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-149">Int64</span></span>   | <span data-ttu-id="79d30-150">Количество сообщений, которые понравилось в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="79d30-150">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="79d30-151">Ексчанжемаилбокстоталитемкаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-151">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="79d30-152">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-152">Int64</span></span>   | <span data-ttu-id="79d30-153">Количество элементов в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="79d30-153">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="79d30-154">Ексчанжемаилбокссторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="79d30-154">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="79d30-155">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-155">Int64</span></span>   | <span data-ttu-id="79d30-156">Хранилище, используемое для почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="79d30-156">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="79d30-157">Шарепоинттоталфилекаунт</span><span class="sxs-lookup"><span data-stu-id="79d30-157">sharePointTotalFileCount</span></span>          | <span data-ttu-id="79d30-158">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-158">Int64</span></span>   | <span data-ttu-id="79d30-159">Общее количество файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="79d30-159">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="79d30-160">Шарепоинтситесторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="79d30-160">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="79d30-161">Int64</span><span class="sxs-lookup"><span data-stu-id="79d30-161">Int64</span></span>   | <span data-ttu-id="79d30-162">Хранилище, используемое сайтом группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="79d30-162">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="79d30-163">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="79d30-163">reportPeriod</span></span>                      | <span data-ttu-id="79d30-164">String</span><span class="sxs-lookup"><span data-stu-id="79d30-164">String</span></span>  | <span data-ttu-id="79d30-165">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="79d30-165">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="79d30-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79d30-166">JSON representation</span></span>

<span data-ttu-id="79d30-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79d30-167">The following is a JSON representation of the resource.</span></span>

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
