---
title: Тип ресурса office365ActiveUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0d0ebd451252766801239e63804b59b9a1747764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966547"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="b143d-103">Тип ресурса office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="b143d-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b143d-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b143d-104">Properties</span></span>

| <span data-ttu-id="b143d-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b143d-105">Property</span></span>          | <span data-ttu-id="b143d-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b143d-106">Type</span></span>   | <span data-ttu-id="b143d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b143d-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="b143d-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="b143d-108">reportRefreshDate</span></span> | <span data-ttu-id="b143d-109">Дата</span><span class="sxs-lookup"><span data-stu-id="b143d-109">Date</span></span>   | <span data-ttu-id="b143d-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="b143d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="b143d-111">Office365</span><span class="sxs-lookup"><span data-stu-id="b143d-111">office365</span></span>         | <span data-ttu-id="b143d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b143d-112">Int64</span></span>  | <span data-ttu-id="b143d-113">Количество активных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="b143d-113">The number of active users in Office 365.</span></span> <span data-ttu-id="b143d-114">Это число включает все активные пользователи в Exchange, OneDrive, SharePoint, Skype для бизнеса, Yammer и Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b143d-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="b143d-115">Определение активных пользователей для каждого продукта можно найти в описании соответствующего свойства.</span><span class="sxs-lookup"><span data-stu-id="b143d-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="b143d-116">теплообменник</span><span class="sxs-lookup"><span data-stu-id="b143d-116">exchange</span></span>          | <span data-ttu-id="b143d-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b143d-117">Int64</span></span>  | <span data-ttu-id="b143d-118">Количество активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b143d-118">The number of active users in Exchange.</span></span> <span data-ttu-id="b143d-119">Любой пользователь, который может читать и отправлять электронную почту, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="b143d-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="b143d-120">oneDrive</span><span class="sxs-lookup"><span data-stu-id="b143d-120">oneDrive</span></span>          | <span data-ttu-id="b143d-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b143d-121">Int64</span></span>  | <span data-ttu-id="b143d-122">Количество активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b143d-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="b143d-123">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, или синхронизированные файлы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="b143d-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="b143d-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="b143d-124">sharePoint</span></span>        | <span data-ttu-id="b143d-125">Int64</span><span class="sxs-lookup"><span data-stu-id="b143d-125">Int64</span></span>  | <span data-ttu-id="b143d-126">Количество активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b143d-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="b143d-127">Любой пользователь, просматривающий или изменяющий файлы, внутренние и внешние файлы, синхронизированные файлы или просмотренные страницы SharePoint, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="b143d-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="b143d-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="b143d-128">skypeForBusiness</span></span>  | <span data-ttu-id="b143d-129">Int64</span><span class="sxs-lookup"><span data-stu-id="b143d-129">Int64</span></span>  | <span data-ttu-id="b143d-130">Количество активных пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b143d-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="b143d-131">Любой пользователь, который организует или принимал участие в конференциях или присоединяет одноранговые сеансы, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="b143d-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="b143d-132">Yammer</span><span class="sxs-lookup"><span data-stu-id="b143d-132">yammer</span></span>            | <span data-ttu-id="b143d-133">Int64</span><span class="sxs-lookup"><span data-stu-id="b143d-133">Int64</span></span>  | <span data-ttu-id="b143d-134">Количество активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="b143d-134">The number of active users in Yammer.</span></span> <span data-ttu-id="b143d-135">Любой пользователь, который может отправлять, читать и аналогичные сообщения, считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="b143d-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="b143d-136">Teams</span><span class="sxs-lookup"><span data-stu-id="b143d-136">teams</span></span>             | <span data-ttu-id="b143d-137">Int64</span><span class="sxs-lookup"><span data-stu-id="b143d-137">Int64</span></span>  | <span data-ttu-id="b143d-138">Количество активных пользователей в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b143d-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="b143d-139">Любой пользователь, который опубликовал сообщения в каналах группы, отправил сообщения в сеансах частного чата или участие в собраниях или вызовах считается активным пользователем.</span><span class="sxs-lookup"><span data-stu-id="b143d-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="b143d-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="b143d-140">reportDate</span></span>        | <span data-ttu-id="b143d-141">Дата</span><span class="sxs-lookup"><span data-stu-id="b143d-141">Date</span></span>   | <span data-ttu-id="b143d-142">Дата, когда число пользователей было активно.</span><span class="sxs-lookup"><span data-stu-id="b143d-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="b143d-143">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="b143d-143">reportPeriod</span></span>      | <span data-ttu-id="b143d-144">String</span><span class="sxs-lookup"><span data-stu-id="b143d-144">String</span></span> | <span data-ttu-id="b143d-145">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="b143d-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b143d-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b143d-146">JSON representation</span></span>

<span data-ttu-id="b143d-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b143d-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
