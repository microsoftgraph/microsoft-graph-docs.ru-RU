---
title: Тип ресурса office365ServicesUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 5958ab3cb05767465b0866078d378208f1b466e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009470"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="2eb0f-103">Тип ресурса office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="2eb0f-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2eb0f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2eb0f-104">Properties</span></span>

| <span data-ttu-id="2eb0f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2eb0f-105">Property</span></span>                 | <span data-ttu-id="2eb0f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2eb0f-106">Type</span></span>   | <span data-ttu-id="2eb0f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2eb0f-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2eb0f-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="2eb0f-108">reportRefreshDate</span></span>        | <span data-ttu-id="2eb0f-109">Дата</span><span class="sxs-lookup"><span data-stu-id="2eb0f-109">Date</span></span>   | <span data-ttu-id="2eb0f-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2eb0f-111">Ексчанжеактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-111">exchangeActive</span></span>           | <span data-ttu-id="2eb0f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-112">Int64</span></span>  | <span data-ttu-id="2eb0f-113">Количество активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-113">The number of active users on Exchange.</span></span> <span data-ttu-id="2eb0f-114">Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="2eb0f-115">Ексчанжеинактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-115">exchangeInactive</span></span>         | <span data-ttu-id="2eb0f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-116">Int64</span></span>  | <span data-ttu-id="2eb0f-117">Количество неактивных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="2eb0f-118">Онедривеактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-118">oneDriveActive</span></span>           | <span data-ttu-id="2eb0f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-119">Int64</span></span>  | <span data-ttu-id="2eb0f-120">Количество активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="2eb0f-121">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, или синхронизированные файлы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="2eb0f-122">Онедривеинактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-122">oneDriveInactive</span></span>         | <span data-ttu-id="2eb0f-123">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-123">Int64</span></span>  | <span data-ttu-id="2eb0f-124">Количество неактивных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="2eb0f-125">Шарепоинтактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-125">sharePointActive</span></span>         | <span data-ttu-id="2eb0f-126">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-126">Int64</span></span>  | <span data-ttu-id="2eb0f-127">Количество активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="2eb0f-128">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, синхронизированные файлы или просмотренные страницы SharePoint, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="2eb0f-129">Шарепоинтинактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-129">sharePointInactive</span></span>       | <span data-ttu-id="2eb0f-130">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-130">Int64</span></span>  | <span data-ttu-id="2eb0f-131">Количество неактивных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="2eb0f-132">Скипефорбусинессактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="2eb0f-133">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-133">Int64</span></span>  | <span data-ttu-id="2eb0f-134">Количество активных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="2eb0f-135">Любой пользователь, который организует или принимал участие в конференциях или присоединяет одноранговые сеансы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="2eb0f-136">Скипефорбусинессинактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="2eb0f-137">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-137">Int64</span></span>  | <span data-ttu-id="2eb0f-138">Количество неактивных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="2eb0f-139">Яммерактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-139">yammerActive</span></span>             | <span data-ttu-id="2eb0f-140">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-140">Int64</span></span>  | <span data-ttu-id="2eb0f-141">Количество активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-141">The number of active users on Yammer.</span></span> <span data-ttu-id="2eb0f-142">Любой пользователь, который может отправлять, читать и аналогичные сообщения, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="2eb0f-143">Яммеринактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-143">yammerInactive</span></span>           | <span data-ttu-id="2eb0f-144">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-144">Int64</span></span>  | <span data-ttu-id="2eb0f-145">Количество неактивных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="2eb0f-146">Теамсактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-146">teamsActive</span></span>              | <span data-ttu-id="2eb0f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-147">Int64</span></span>  | <span data-ttu-id="2eb0f-148">Количество активных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="2eb0f-149">Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах частного чата или участие в собраниях или вызовах считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="2eb0f-150">Теамсинактиве</span><span class="sxs-lookup"><span data-stu-id="2eb0f-150">teamsInactive</span></span>            | <span data-ttu-id="2eb0f-151">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-151">Int64</span></span>  | <span data-ttu-id="2eb0f-152">Количество неактивных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="2eb0f-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="2eb0f-153">office365Active</span></span>          | <span data-ttu-id="2eb0f-154">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-154">Int64</span></span>  | <span data-ttu-id="2eb0f-155">Количество активных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="2eb0f-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="2eb0f-156">office365Inactive</span></span>        | <span data-ttu-id="2eb0f-157">Int64</span><span class="sxs-lookup"><span data-stu-id="2eb0f-157">Int64</span></span>  | <span data-ttu-id="2eb0f-158">Количество неактивных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="2eb0f-159">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="2eb0f-159">reportPeriod</span></span>             | <span data-ttu-id="2eb0f-160">String</span><span class="sxs-lookup"><span data-stu-id="2eb0f-160">String</span></span> | <span data-ttu-id="2eb0f-161">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2eb0f-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2eb0f-162">JSON representation</span></span>

<span data-ttu-id="2eb0f-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2eb0f-163">The following is a JSON representation of the resource.</span></span>

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
