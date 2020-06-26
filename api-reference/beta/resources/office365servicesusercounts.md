---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8600e79d425d15746fd7015adea98eb49a8a3c82
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896555"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="f5455-103">Тип ресурса office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="f5455-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="f5455-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5455-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f5455-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5455-105">Properties</span></span>

| <span data-ttu-id="f5455-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5455-106">Property</span></span>                 | <span data-ttu-id="f5455-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f5455-107">Type</span></span>   | <span data-ttu-id="f5455-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f5455-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="f5455-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="f5455-109">reportRefreshDate</span></span>        | <span data-ttu-id="f5455-110">Дата</span><span class="sxs-lookup"><span data-stu-id="f5455-110">Date</span></span>   | <span data-ttu-id="f5455-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="f5455-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="f5455-112">ексчанжеактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-112">exchangeActive</span></span>           | <span data-ttu-id="f5455-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-113">Int64</span></span>  | <span data-ttu-id="f5455-114">Количество активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5455-114">The number of active users on Exchange.</span></span> <span data-ttu-id="f5455-115">Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="f5455-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="f5455-116">ексчанжеинактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-116">exchangeInactive</span></span>         | <span data-ttu-id="f5455-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-117">Int64</span></span>  | <span data-ttu-id="f5455-118">Количество неактивных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f5455-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="f5455-119">онедривеактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-119">oneDriveActive</span></span>           | <span data-ttu-id="f5455-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-120">Int64</span></span>  | <span data-ttu-id="f5455-121">Количество активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f5455-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="f5455-122">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, или синхронизированные файлы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="f5455-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="f5455-123">онедривеинактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-123">oneDriveInactive</span></span>         | <span data-ttu-id="f5455-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-124">Int64</span></span>  | <span data-ttu-id="f5455-125">Количество неактивных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f5455-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="f5455-126">шарепоинтактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-126">sharePointActive</span></span>         | <span data-ttu-id="f5455-127">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-127">Int64</span></span>  | <span data-ttu-id="f5455-128">Количество активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f5455-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="f5455-129">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, синхронизированные файлы или просмотренные страницы SharePoint, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="f5455-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="f5455-130">шарепоинтинактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-130">sharePointInactive</span></span>       | <span data-ttu-id="f5455-131">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-131">Int64</span></span>  | <span data-ttu-id="f5455-132">Количество неактивных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f5455-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="f5455-133">скипефорбусинессактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="f5455-134">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-134">Int64</span></span>  | <span data-ttu-id="f5455-135">Количество активных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f5455-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="f5455-136">Любой пользователь, который организует или принимал участие в конференциях или присоединяет одноранговые сеансы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="f5455-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="f5455-137">скипефорбусинессинактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="f5455-138">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-138">Int64</span></span>  | <span data-ttu-id="f5455-139">Количество неактивных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f5455-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="f5455-140">яммерактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-140">yammerActive</span></span>             | <span data-ttu-id="f5455-141">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-141">Int64</span></span>  | <span data-ttu-id="f5455-142">Количество активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="f5455-142">The number of active users on Yammer.</span></span> <span data-ttu-id="f5455-143">Любой пользователь, который может отправлять, читать и аналогичные сообщения, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="f5455-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="f5455-144">яммеринактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-144">yammerInactive</span></span>           | <span data-ttu-id="f5455-145">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-145">Int64</span></span>  | <span data-ttu-id="f5455-146">Количество неактивных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="f5455-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="f5455-147">теамсактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-147">teamsActive</span></span>              | <span data-ttu-id="f5455-148">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-148">Int64</span></span>  | <span data-ttu-id="f5455-149">Количество активных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f5455-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="f5455-150">Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах частного чата или участие в собраниях или вызовах считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="f5455-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="f5455-151">теамсинактиве</span><span class="sxs-lookup"><span data-stu-id="f5455-151">teamsInactive</span></span>            | <span data-ttu-id="f5455-152">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-152">Int64</span></span>  | <span data-ttu-id="f5455-153">Количество неактивных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f5455-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="f5455-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="f5455-154">office365Active</span></span>          | <span data-ttu-id="f5455-155">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-155">Int64</span></span>  | <span data-ttu-id="f5455-156">Количество активных пользователей в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f5455-156">The number of active users on Microsoft 365.</span></span>   |
| <span data-ttu-id="f5455-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="f5455-157">office365Inactive</span></span>        | <span data-ttu-id="f5455-158">Int64</span><span class="sxs-lookup"><span data-stu-id="f5455-158">Int64</span></span>  | <span data-ttu-id="f5455-159">Количество неактивных пользователей в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f5455-159">The number of inactive users on Microsoft 365.</span></span>     |
| <span data-ttu-id="f5455-160">репортпериод</span><span class="sxs-lookup"><span data-stu-id="f5455-160">reportPeriod</span></span>             | <span data-ttu-id="f5455-161">String</span><span class="sxs-lookup"><span data-stu-id="f5455-161">String</span></span> | <span data-ttu-id="f5455-162">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="f5455-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f5455-163">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f5455-163">JSON representation</span></span>

<span data-ttu-id="f5455-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5455-164">The following is a JSON representation of the resource.</span></span>

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
