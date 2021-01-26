---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 1f4f26e141dc25e1e5e249ad116bc9a988274f18
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981503"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="27e4c-103">Тип ресурса office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="27e4c-103">office365GroupsActivityFileCounts resource type</span></span>

<span data-ttu-id="27e4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27e4c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="27e4c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="27e4c-105">Properties</span></span>

| <span data-ttu-id="27e4c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="27e4c-106">Property</span></span>          | <span data-ttu-id="27e4c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="27e4c-107">Type</span></span>   | <span data-ttu-id="27e4c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27e4c-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="27e4c-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="27e4c-109">reportRefreshDate</span></span> | <span data-ttu-id="27e4c-110">Дата</span><span class="sxs-lookup"><span data-stu-id="27e4c-110">Date</span></span>   | <span data-ttu-id="27e4c-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="27e4c-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="27e4c-112">total</span><span class="sxs-lookup"><span data-stu-id="27e4c-112">total</span></span>             | <span data-ttu-id="27e4c-113">Int64</span><span class="sxs-lookup"><span data-stu-id="27e4c-113">Int64</span></span>  | <span data-ttu-id="27e4c-114">Общее количество файлов в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="27e4c-114">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="27e4c-115">active</span><span class="sxs-lookup"><span data-stu-id="27e4c-115">active</span></span>            | <span data-ttu-id="27e4c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="27e4c-116">Int64</span></span>  | <span data-ttu-id="27e4c-117">Количество файлов, которые просматривались, редактируются, совместно или синхронизированы в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="27e4c-117">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="27e4c-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="27e4c-118">reportDate</span></span>        | <span data-ttu-id="27e4c-119">Дата</span><span class="sxs-lookup"><span data-stu-id="27e4c-119">Date</span></span>   | <span data-ttu-id="27e4c-120">Дата, когда на сайте SharePoint группы было активно несколько файлов.</span><span class="sxs-lookup"><span data-stu-id="27e4c-120">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="27e4c-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="27e4c-121">reportPeriod</span></span>      | <span data-ttu-id="27e4c-122">String</span><span class="sxs-lookup"><span data-stu-id="27e4c-122">String</span></span> | <span data-ttu-id="27e4c-123">Количество дней в отчете.</span><span class="sxs-lookup"><span data-stu-id="27e4c-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="27e4c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27e4c-124">JSON representation</span></span>

<span data-ttu-id="27e4c-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27e4c-125">The following is a JSON representation of the resource.</span></span>

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
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


