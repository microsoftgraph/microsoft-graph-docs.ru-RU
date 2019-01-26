---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 89ac23b89730ec98515d6d0d3c06867e57b19ed1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575578"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="eeedc-103">Тип ресурса office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="eeedc-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="eeedc-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="eeedc-104">Properties</span></span>

| <span data-ttu-id="eeedc-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeedc-105">Property</span></span>          | <span data-ttu-id="eeedc-106">Тип</span><span class="sxs-lookup"><span data-stu-id="eeedc-106">Type</span></span>   | <span data-ttu-id="eeedc-107">Описание</span><span class="sxs-lookup"><span data-stu-id="eeedc-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="eeedc-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="eeedc-108">reportRefreshDate</span></span> | <span data-ttu-id="eeedc-109">Date</span><span class="sxs-lookup"><span data-stu-id="eeedc-109">Date</span></span>   | <span data-ttu-id="eeedc-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="eeedc-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="eeedc-111">total</span><span class="sxs-lookup"><span data-stu-id="eeedc-111">total</span></span>             | <span data-ttu-id="eeedc-112">Int64</span><span class="sxs-lookup"><span data-stu-id="eeedc-112">Int64</span></span>  | <span data-ttu-id="eeedc-113">Общее число файлов в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="eeedc-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="eeedc-114">активных</span><span class="sxs-lookup"><span data-stu-id="eeedc-114">active</span></span>            | <span data-ttu-id="eeedc-115">Int64</span><span class="sxs-lookup"><span data-stu-id="eeedc-115">Int64</span></span>  | <span data-ttu-id="eeedc-116">Число файлов, которые были просматривать, редактировать, общих или синхронизирован в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="eeedc-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="eeedc-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="eeedc-117">reportDate</span></span>        | <span data-ttu-id="eeedc-118">Date</span><span class="sxs-lookup"><span data-stu-id="eeedc-118">Date</span></span>   | <span data-ttu-id="eeedc-119">Дата, на котором количество файлов были активны на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eeedc-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="eeedc-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="eeedc-120">reportPeriod</span></span>      | <span data-ttu-id="eeedc-121">Строка</span><span class="sxs-lookup"><span data-stu-id="eeedc-121">String</span></span> | <span data-ttu-id="eeedc-122">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="eeedc-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="eeedc-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eeedc-123">JSON representation</span></span>

<span data-ttu-id="eeedc-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeedc-124">The following is a JSON representation of the resource.</span></span>

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
