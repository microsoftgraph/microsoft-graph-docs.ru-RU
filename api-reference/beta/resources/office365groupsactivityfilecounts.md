---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819188"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="d70aa-103">Тип ресурса office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="d70aa-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d70aa-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d70aa-104">Properties</span></span>

| <span data-ttu-id="d70aa-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d70aa-105">Property</span></span>          | <span data-ttu-id="d70aa-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d70aa-106">Type</span></span>   | <span data-ttu-id="d70aa-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d70aa-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d70aa-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d70aa-108">reportRefreshDate</span></span> | <span data-ttu-id="d70aa-109">Date</span><span class="sxs-lookup"><span data-stu-id="d70aa-109">Date</span></span>   | <span data-ttu-id="d70aa-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="d70aa-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d70aa-111">total</span><span class="sxs-lookup"><span data-stu-id="d70aa-111">total</span></span>             | <span data-ttu-id="d70aa-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d70aa-112">Int64</span></span>  | <span data-ttu-id="d70aa-113">Общее число файлов в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="d70aa-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="d70aa-114">активных</span><span class="sxs-lookup"><span data-stu-id="d70aa-114">active</span></span>            | <span data-ttu-id="d70aa-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d70aa-115">Int64</span></span>  | <span data-ttu-id="d70aa-116">Число файлов, которые были просматривать, редактировать, общих или синхронизирован в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="d70aa-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="d70aa-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="d70aa-117">reportDate</span></span>        | <span data-ttu-id="d70aa-118">Date</span><span class="sxs-lookup"><span data-stu-id="d70aa-118">Date</span></span>   | <span data-ttu-id="d70aa-119">Дата, на котором количество файлов были активны на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d70aa-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="d70aa-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d70aa-120">reportPeriod</span></span>      | <span data-ttu-id="d70aa-121">Строка</span><span class="sxs-lookup"><span data-stu-id="d70aa-121">String</span></span> | <span data-ttu-id="d70aa-122">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="d70aa-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d70aa-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d70aa-123">JSON representation</span></span>

<span data-ttu-id="d70aa-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d70aa-124">The following is a JSON representation of the resource.</span></span>

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
