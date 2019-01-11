---
title: Тип ресурса office365ActiveUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 887f9b08d7f46aac023fbd0f34e6174e5f422760
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882721"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="d2390-103">Тип ресурса office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="d2390-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d2390-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2390-104">Properties</span></span>

| <span data-ttu-id="d2390-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2390-105">Property</span></span>          | <span data-ttu-id="d2390-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d2390-106">Type</span></span>   | <span data-ttu-id="d2390-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d2390-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d2390-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d2390-108">reportRefreshDate</span></span> | <span data-ttu-id="d2390-109">Date</span><span class="sxs-lookup"><span data-stu-id="d2390-109">Date</span></span>   | <span data-ttu-id="d2390-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="d2390-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d2390-111">Office 365</span><span class="sxs-lookup"><span data-stu-id="d2390-111">office365</span></span>         | <span data-ttu-id="d2390-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d2390-112">Int64</span></span>  | <span data-ttu-id="d2390-113">Число активных пользователей в Office 365.</span><span class="sxs-lookup"><span data-stu-id="d2390-113">The number of active users in Office 365.</span></span> <span data-ttu-id="d2390-114">Эта цифра включает в себя всех активных пользователей в Exchange, OneDrive, SharePoint, Скайп для бизнеса, Yammer и группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d2390-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="d2390-115">Определение активного пользователя можно найти для каждого продукта в описании соответствующих свойств.</span><span class="sxs-lookup"><span data-stu-id="d2390-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="d2390-116">Exchange</span><span class="sxs-lookup"><span data-stu-id="d2390-116">exchange</span></span>          | <span data-ttu-id="d2390-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d2390-117">Int64</span></span>  | <span data-ttu-id="d2390-118">Число активных пользователей в Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2390-118">The number of active users in Exchange.</span></span> <span data-ttu-id="d2390-119">Любой пользователь, который можно читать и отправлять электронную почту считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2390-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="d2390-120">oneDrive</span><span class="sxs-lookup"><span data-stu-id="d2390-120">oneDrive</span></span>          | <span data-ttu-id="d2390-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d2390-121">Int64</span></span>  | <span data-ttu-id="d2390-122">Число активных пользователей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d2390-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="d2390-123">Любой пользователь, просматривать или изменять файлы, общих файлов во внутреннем или внешнем ресурсе или синхронизирован файлы считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2390-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="d2390-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="d2390-124">sharePoint</span></span>        | <span data-ttu-id="d2390-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d2390-125">Int64</span></span>  | <span data-ttu-id="d2390-126">Число активных пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d2390-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="d2390-127">Любой пользователь, просматривать или изменять файлы, общих файлов во внутренней сети или извне, синхронизированные файлы или просматривать страницы SharePoint считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2390-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="d2390-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="d2390-128">skypeForBusiness</span></span>  | <span data-ttu-id="d2390-129">Int64</span><span class="sxs-lookup"><span data-stu-id="d2390-129">Int64</span></span>  | <span data-ttu-id="d2390-130">Число активных пользователей в Скайп для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d2390-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="d2390-131">Любой пользователь, который организовал принявших участие в конференциях или в состав peer-to-peer sessions считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2390-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="d2390-132">Yammer</span><span class="sxs-lookup"><span data-stu-id="d2390-132">yammer</span></span>            | <span data-ttu-id="d2390-133">Int64</span><span class="sxs-lookup"><span data-stu-id="d2390-133">Int64</span></span>  | <span data-ttu-id="d2390-134">Число активных пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="d2390-134">The number of active users in Yammer.</span></span> <span data-ttu-id="d2390-135">Любой пользователь, который можно публиковать, чтение или как сообщения считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2390-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="d2390-136">группы</span><span class="sxs-lookup"><span data-stu-id="d2390-136">teams</span></span>             | <span data-ttu-id="d2390-137">Int64</span><span class="sxs-lookup"><span data-stu-id="d2390-137">Int64</span></span>  | <span data-ttu-id="d2390-138">Число активных пользователей в группы Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d2390-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="d2390-139">Любой пользователь, который сообщений, помещенных в каналы группы, отправленных сообщений в сеансах частной беседы или являлся участником собрания или вызовы считается активного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2390-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="d2390-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="d2390-140">reportDate</span></span>        | <span data-ttu-id="d2390-141">Date</span><span class="sxs-lookup"><span data-stu-id="d2390-141">Date</span></span>   | <span data-ttu-id="d2390-142">Дата, на котором выполнялись число пользователей.</span><span class="sxs-lookup"><span data-stu-id="d2390-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="d2390-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d2390-143">reportPeriod</span></span>      | <span data-ttu-id="d2390-144">Строка</span><span class="sxs-lookup"><span data-stu-id="d2390-144">String</span></span> | <span data-ttu-id="d2390-145">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="d2390-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d2390-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2390-146">JSON representation</span></span>

<span data-ttu-id="d2390-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2390-147">The following is a JSON representation of the resource.</span></span>

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
