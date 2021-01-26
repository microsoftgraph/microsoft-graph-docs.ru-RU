---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: ad2610f5cbd3aae56651a0a5651e4ee4319b3bb2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981496"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="1f199-103">Тип ресурса office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="1f199-103">office365GroupsActivityGroupCounts resource type</span></span>

<span data-ttu-id="1f199-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f199-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="1f199-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f199-105">Properties</span></span>

| <span data-ttu-id="1f199-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f199-106">Property</span></span>          | <span data-ttu-id="1f199-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1f199-107">Type</span></span>   | <span data-ttu-id="1f199-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1f199-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="1f199-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1f199-109">reportRefreshDate</span></span> | <span data-ttu-id="1f199-110">Дата</span><span class="sxs-lookup"><span data-stu-id="1f199-110">Date</span></span>   | <span data-ttu-id="1f199-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="1f199-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="1f199-112">total</span><span class="sxs-lookup"><span data-stu-id="1f199-112">total</span></span>             | <span data-ttu-id="1f199-113">Int64</span><span class="sxs-lookup"><span data-stu-id="1f199-113">Int64</span></span>  | <span data-ttu-id="1f199-114">Общее количество групп.</span><span class="sxs-lookup"><span data-stu-id="1f199-114">The total number of groups.</span></span>              |
| <span data-ttu-id="1f199-115">active</span><span class="sxs-lookup"><span data-stu-id="1f199-115">active</span></span>            | <span data-ttu-id="1f199-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1f199-116">Int64</span></span>  | <span data-ttu-id="1f199-117">Количество активных групп.</span><span class="sxs-lookup"><span data-stu-id="1f199-117">The number of active groups.</span></span> <span data-ttu-id="1f199-118">Группа считается активной при любом из следующих действий: почтовый ящик группы, полученный по электронной почте; просматриваются, редактируются, совместно или синхронизируются файлы в библиотеке документов SharePoint; просматривались пользователем страницы SharePoint; пользователи опубликовали, прочитали или понравились сообщения в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="1f199-118">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="1f199-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="1f199-119">reportDate</span></span>        | <span data-ttu-id="1f199-120">Дата</span><span class="sxs-lookup"><span data-stu-id="1f199-120">Date</span></span>   | <span data-ttu-id="1f199-121">Дата, когда было активно несколько групп.</span><span class="sxs-lookup"><span data-stu-id="1f199-121">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="1f199-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1f199-122">reportPeriod</span></span>      | <span data-ttu-id="1f199-123">String</span><span class="sxs-lookup"><span data-stu-id="1f199-123">String</span></span> | <span data-ttu-id="1f199-124">Количество дней в отчете.</span><span class="sxs-lookup"><span data-stu-id="1f199-124">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="1f199-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f199-125">JSON representation</span></span>

<span data-ttu-id="1f199-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f199-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


