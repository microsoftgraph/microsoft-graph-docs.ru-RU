---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 89ac23b89730ec98515d6d0d3c06867e57b19ed1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457076"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="2e74f-103">Тип ресурса office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="2e74f-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2e74f-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e74f-104">Properties</span></span>

| <span data-ttu-id="2e74f-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e74f-105">Property</span></span>          | <span data-ttu-id="2e74f-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2e74f-106">Type</span></span>   | <span data-ttu-id="2e74f-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2e74f-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2e74f-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="2e74f-108">reportRefreshDate</span></span> | <span data-ttu-id="2e74f-109">Дата</span><span class="sxs-lookup"><span data-stu-id="2e74f-109">Date</span></span>   | <span data-ttu-id="2e74f-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="2e74f-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2e74f-111">total</span><span class="sxs-lookup"><span data-stu-id="2e74f-111">total</span></span>             | <span data-ttu-id="2e74f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2e74f-112">Int64</span></span>  | <span data-ttu-id="2e74f-113">Общее количество файлов в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="2e74f-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="2e74f-114">ASP</span><span class="sxs-lookup"><span data-stu-id="2e74f-114">active</span></span>            | <span data-ttu-id="2e74f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2e74f-115">Int64</span></span>  | <span data-ttu-id="2e74f-116">Количество файлов, которые были просмотрены, изменены, предоставлены в общий доступ или синхронизированы в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="2e74f-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="2e74f-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="2e74f-117">reportDate</span></span>        | <span data-ttu-id="2e74f-118">Дата</span><span class="sxs-lookup"><span data-stu-id="2e74f-118">Date</span></span>   | <span data-ttu-id="2e74f-119">Дата, когда число файлов было активно на сайте SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="2e74f-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="2e74f-120">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="2e74f-120">reportPeriod</span></span>      | <span data-ttu-id="2e74f-121">Строка</span><span class="sxs-lookup"><span data-stu-id="2e74f-121">String</span></span> | <span data-ttu-id="2e74f-122">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="2e74f-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2e74f-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e74f-123">JSON representation</span></span>

<span data-ttu-id="2e74f-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e74f-124">The following is a JSON representation of the resource.</span></span>

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
