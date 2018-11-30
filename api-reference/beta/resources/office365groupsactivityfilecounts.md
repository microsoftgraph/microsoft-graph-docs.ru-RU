---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: eb2d967108d4f75064b91670ae43fb7a2dd7ce7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076002"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="60449-103">Тип ресурса office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="60449-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="60449-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="60449-104">Properties</span></span>

| <span data-ttu-id="60449-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="60449-105">Property</span></span>          | <span data-ttu-id="60449-106">Тип</span><span class="sxs-lookup"><span data-stu-id="60449-106">Type</span></span>   | <span data-ttu-id="60449-107">Description</span><span class="sxs-lookup"><span data-stu-id="60449-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="60449-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="60449-108">reportRefreshDate</span></span> | <span data-ttu-id="60449-109">Date</span><span class="sxs-lookup"><span data-stu-id="60449-109">Date</span></span>   | <span data-ttu-id="60449-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="60449-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="60449-111">total</span><span class="sxs-lookup"><span data-stu-id="60449-111">total</span></span>             | <span data-ttu-id="60449-112">Int64</span><span class="sxs-lookup"><span data-stu-id="60449-112">Int64</span></span>  | <span data-ttu-id="60449-113">Общее число файлов в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="60449-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="60449-114">активных</span><span class="sxs-lookup"><span data-stu-id="60449-114">active</span></span>            | <span data-ttu-id="60449-115">Int64</span><span class="sxs-lookup"><span data-stu-id="60449-115">Int64</span></span>  | <span data-ttu-id="60449-116">Число файлов, которые были просматривать, редактировать, общих или синхронизирован в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="60449-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="60449-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="60449-117">reportDate</span></span>        | <span data-ttu-id="60449-118">Date</span><span class="sxs-lookup"><span data-stu-id="60449-118">Date</span></span>   | <span data-ttu-id="60449-119">Дата, на котором количество файлов были активны на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="60449-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="60449-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="60449-120">reportPeriod</span></span>      | <span data-ttu-id="60449-121">String</span><span class="sxs-lookup"><span data-stu-id="60449-121">String</span></span> | <span data-ttu-id="60449-122">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="60449-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="60449-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60449-123">JSON representation</span></span>

<span data-ttu-id="60449-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60449-124">The following is a JSON representation of the resource.</span></span>

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
