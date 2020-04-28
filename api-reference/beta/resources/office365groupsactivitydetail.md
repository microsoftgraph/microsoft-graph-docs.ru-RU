---
title: Тип ресурса office365GroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d517763fdfcbf046c36fc944d229b9a15b0cb8fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522451"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="f0393-103">Тип ресурса office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="f0393-103">office365GroupsActivityDetail resource type</span></span>

<span data-ttu-id="f0393-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0393-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f0393-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0393-105">Properties</span></span>

| <span data-ttu-id="f0393-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0393-106">Property</span></span>                          | <span data-ttu-id="f0393-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f0393-107">Type</span></span>    | <span data-ttu-id="f0393-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f0393-108">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="f0393-109">groupId</span><span class="sxs-lookup"><span data-stu-id="f0393-109">groupId</span></span>                           | <span data-ttu-id="f0393-110">String</span><span class="sxs-lookup"><span data-stu-id="f0393-110">String</span></span>  | <span data-ttu-id="f0393-111">Идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="f0393-111">The group id.</span></span>          |
| <span data-ttu-id="f0393-112">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="f0393-112">reportRefreshDate</span></span>                 | <span data-ttu-id="f0393-113">Дата</span><span class="sxs-lookup"><span data-stu-id="f0393-113">Date</span></span>    | <span data-ttu-id="f0393-114">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="f0393-114">The latest date of the content.</span></span>          |
| <span data-ttu-id="f0393-115">граупдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="f0393-115">groupDisplayName</span></span>                  | <span data-ttu-id="f0393-116">String</span><span class="sxs-lookup"><span data-stu-id="f0393-116">String</span></span>  | <span data-ttu-id="f0393-117">Отображаемое имя группы.</span><span class="sxs-lookup"><span data-stu-id="f0393-117">The display name of the group.</span></span>           |
| <span data-ttu-id="f0393-118">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f0393-118">isDeleted</span></span>                         | <span data-ttu-id="f0393-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0393-119">Boolean</span></span> | <span data-ttu-id="f0393-120">Указывает, был ли этот пользователь удален или обратимо удален.</span><span class="sxs-lookup"><span data-stu-id="f0393-120">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="f0393-121">овнерпринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="f0393-121">ownerPrincipalName</span></span>                | <span data-ttu-id="f0393-122">String</span><span class="sxs-lookup"><span data-stu-id="f0393-122">String</span></span>  | <span data-ttu-id="f0393-123">Имя участника владельца группы.</span><span class="sxs-lookup"><span data-stu-id="f0393-123">The group owner principal name.</span></span>          |
| <span data-ttu-id="f0393-124">ластактивитидате</span><span class="sxs-lookup"><span data-stu-id="f0393-124">lastActivityDate</span></span>                  | <span data-ttu-id="f0393-125">Дата</span><span class="sxs-lookup"><span data-stu-id="f0393-125">Date</span></span>    | <span data-ttu-id="f0393-126">Дата последнего действия для следующих сценариев: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="f0393-126">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="f0393-127">groupType</span><span class="sxs-lookup"><span data-stu-id="f0393-127">groupType</span></span>                         | <span data-ttu-id="f0393-128">String</span><span class="sxs-lookup"><span data-stu-id="f0393-128">String</span></span>  | <span data-ttu-id="f0393-129">Тип группы.</span><span class="sxs-lookup"><span data-stu-id="f0393-129">The group type.</span></span> <span data-ttu-id="f0393-130">Возможные значения: **Public** или **Private**.</span><span class="sxs-lookup"><span data-stu-id="f0393-130">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="f0393-131">мемберкаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-131">memberCount</span></span>                       | <span data-ttu-id="f0393-132">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-132">Int64</span></span>   | <span data-ttu-id="f0393-133">Число участников группы.</span><span class="sxs-lookup"><span data-stu-id="f0393-133">The group member count.</span></span>                  |
| <span data-ttu-id="f0393-134">екстерналмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-134">externalMemberCount</span></span>               | <span data-ttu-id="f0393-135">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-135">Int64</span></span>   | <span data-ttu-id="f0393-136">Количество внешних участников группы.</span><span class="sxs-lookup"><span data-stu-id="f0393-136">The group external member count.</span></span>         |
| <span data-ttu-id="f0393-137">ексчанжерецеиведемаилкаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-137">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="f0393-138">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-138">Int64</span></span>   | <span data-ttu-id="f0393-139">Количество сообщений электронной почты, принимаемых группового почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f0393-139">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="f0393-140">шарепоинтактивефилекаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-140">sharePointActiveFileCount</span></span>         | <span data-ttu-id="f0393-141">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-141">Int64</span></span>   | <span data-ttu-id="f0393-142">Количество активных файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f0393-142">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="f0393-143">яммерпостедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-143">yammerPostedMessageCount</span></span>          | <span data-ttu-id="f0393-144">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-144">Int64</span></span>   | <span data-ttu-id="f0393-145">Количество сообщений, отправленных в группы Yammer.</span><span class="sxs-lookup"><span data-stu-id="f0393-145">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="f0393-146">яммерреадмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-146">yammerReadMessageCount</span></span>            | <span data-ttu-id="f0393-147">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-147">Int64</span></span>   | <span data-ttu-id="f0393-148">Количество сообщений, прочитанных в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="f0393-148">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="f0393-149">яммерликедмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-149">yammerLikedMessageCount</span></span>           | <span data-ttu-id="f0393-150">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-150">Int64</span></span>   | <span data-ttu-id="f0393-151">Количество сообщений, которые понравилось в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="f0393-151">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="f0393-152">ексчанжемаилбокстоталитемкаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-152">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="f0393-153">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-153">Int64</span></span>   | <span data-ttu-id="f0393-154">Количество элементов в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="f0393-154">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="f0393-155">ексчанжемаилбокссторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="f0393-155">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="f0393-156">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-156">Int64</span></span>   | <span data-ttu-id="f0393-157">Хранилище, используемое для почтового ящика группы.</span><span class="sxs-lookup"><span data-stu-id="f0393-157">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="f0393-158">шарепоинттоталфилекаунт</span><span class="sxs-lookup"><span data-stu-id="f0393-158">sharePointTotalFileCount</span></span>          | <span data-ttu-id="f0393-159">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-159">Int64</span></span>   | <span data-ttu-id="f0393-160">Общее количество файлов на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f0393-160">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="f0393-161">шарепоинтситесторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="f0393-161">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="f0393-162">Int64</span><span class="sxs-lookup"><span data-stu-id="f0393-162">Int64</span></span>   | <span data-ttu-id="f0393-163">Хранилище, используемое сайтом группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f0393-163">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="f0393-164">репортпериод</span><span class="sxs-lookup"><span data-stu-id="f0393-164">reportPeriod</span></span>                      | <span data-ttu-id="f0393-165">String</span><span class="sxs-lookup"><span data-stu-id="f0393-165">String</span></span>  | <span data-ttu-id="f0393-166">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="f0393-166">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f0393-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0393-167">JSON representation</span></span>

<span data-ttu-id="f0393-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0393-168">The following is a JSON representation of the resource.</span></span>

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
