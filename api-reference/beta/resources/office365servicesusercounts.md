---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0deb5eceb31ca3453c1cc5f29ae669f7053738c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522423"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="207f2-103">Тип ресурса office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="207f2-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="207f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="207f2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="207f2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="207f2-105">Properties</span></span>

| <span data-ttu-id="207f2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="207f2-106">Property</span></span>                 | <span data-ttu-id="207f2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="207f2-107">Type</span></span>   | <span data-ttu-id="207f2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="207f2-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="207f2-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="207f2-109">reportRefreshDate</span></span>        | <span data-ttu-id="207f2-110">Дата</span><span class="sxs-lookup"><span data-stu-id="207f2-110">Date</span></span>   | <span data-ttu-id="207f2-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="207f2-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="207f2-112">ексчанжеактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-112">exchangeActive</span></span>           | <span data-ttu-id="207f2-113">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-113">Int64</span></span>  | <span data-ttu-id="207f2-114">Количество активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="207f2-114">The number of active users on Exchange.</span></span> <span data-ttu-id="207f2-115">Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="207f2-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="207f2-116">ексчанжеинактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-116">exchangeInactive</span></span>         | <span data-ttu-id="207f2-117">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-117">Int64</span></span>  | <span data-ttu-id="207f2-118">Количество неактивных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="207f2-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="207f2-119">онедривеактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-119">oneDriveActive</span></span>           | <span data-ttu-id="207f2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-120">Int64</span></span>  | <span data-ttu-id="207f2-121">Количество активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="207f2-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="207f2-122">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, или синхронизированные файлы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="207f2-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="207f2-123">онедривеинактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-123">oneDriveInactive</span></span>         | <span data-ttu-id="207f2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-124">Int64</span></span>  | <span data-ttu-id="207f2-125">Количество неактивных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="207f2-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="207f2-126">шарепоинтактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-126">sharePointActive</span></span>         | <span data-ttu-id="207f2-127">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-127">Int64</span></span>  | <span data-ttu-id="207f2-128">Количество активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="207f2-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="207f2-129">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, синхронизированные файлы или просмотренные страницы SharePoint, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="207f2-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="207f2-130">шарепоинтинактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-130">sharePointInactive</span></span>       | <span data-ttu-id="207f2-131">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-131">Int64</span></span>  | <span data-ttu-id="207f2-132">Количество неактивных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="207f2-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="207f2-133">скипефорбусинессактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="207f2-134">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-134">Int64</span></span>  | <span data-ttu-id="207f2-135">Количество активных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="207f2-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="207f2-136">Любой пользователь, который организует или принимал участие в конференциях или присоединяет одноранговые сеансы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="207f2-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="207f2-137">скипефорбусинессинактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="207f2-138">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-138">Int64</span></span>  | <span data-ttu-id="207f2-139">Количество неактивных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="207f2-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="207f2-140">яммерактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-140">yammerActive</span></span>             | <span data-ttu-id="207f2-141">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-141">Int64</span></span>  | <span data-ttu-id="207f2-142">Количество активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="207f2-142">The number of active users on Yammer.</span></span> <span data-ttu-id="207f2-143">Любой пользователь, который может отправлять, читать и аналогичные сообщения, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="207f2-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="207f2-144">яммеринактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-144">yammerInactive</span></span>           | <span data-ttu-id="207f2-145">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-145">Int64</span></span>  | <span data-ttu-id="207f2-146">Количество неактивных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="207f2-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="207f2-147">теамсактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-147">teamsActive</span></span>              | <span data-ttu-id="207f2-148">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-148">Int64</span></span>  | <span data-ttu-id="207f2-149">Количество активных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="207f2-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="207f2-150">Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах частного чата или участие в собраниях или вызовах считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="207f2-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="207f2-151">теамсинактиве</span><span class="sxs-lookup"><span data-stu-id="207f2-151">teamsInactive</span></span>            | <span data-ttu-id="207f2-152">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-152">Int64</span></span>  | <span data-ttu-id="207f2-153">Количество неактивных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="207f2-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="207f2-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="207f2-154">office365Active</span></span>          | <span data-ttu-id="207f2-155">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-155">Int64</span></span>  | <span data-ttu-id="207f2-156">Количество активных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="207f2-156">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="207f2-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="207f2-157">office365Inactive</span></span>        | <span data-ttu-id="207f2-158">Int64</span><span class="sxs-lookup"><span data-stu-id="207f2-158">Int64</span></span>  | <span data-ttu-id="207f2-159">Количество неактивных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="207f2-159">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="207f2-160">репортпериод</span><span class="sxs-lookup"><span data-stu-id="207f2-160">reportPeriod</span></span>             | <span data-ttu-id="207f2-161">String</span><span class="sxs-lookup"><span data-stu-id="207f2-161">String</span></span> | <span data-ttu-id="207f2-162">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="207f2-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="207f2-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="207f2-163">JSON representation</span></span>

<span data-ttu-id="207f2-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="207f2-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```
