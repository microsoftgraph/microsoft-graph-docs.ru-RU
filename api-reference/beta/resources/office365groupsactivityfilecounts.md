---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8154f24fe36f2c11f3926412c3fcc062be04b5ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966526"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="6f190-103">Тип ресурса office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="6f190-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6f190-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f190-104">Properties</span></span>

| <span data-ttu-id="6f190-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f190-105">Property</span></span>          | <span data-ttu-id="6f190-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6f190-106">Type</span></span>   | <span data-ttu-id="6f190-107">Описание</span><span class="sxs-lookup"><span data-stu-id="6f190-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="6f190-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="6f190-108">reportRefreshDate</span></span> | <span data-ttu-id="6f190-109">Дата</span><span class="sxs-lookup"><span data-stu-id="6f190-109">Date</span></span>   | <span data-ttu-id="6f190-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="6f190-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="6f190-111">total</span><span class="sxs-lookup"><span data-stu-id="6f190-111">total</span></span>             | <span data-ttu-id="6f190-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6f190-112">Int64</span></span>  | <span data-ttu-id="6f190-113">Общее количество файлов в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="6f190-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="6f190-114">ASP</span><span class="sxs-lookup"><span data-stu-id="6f190-114">active</span></span>            | <span data-ttu-id="6f190-115">Int64</span><span class="sxs-lookup"><span data-stu-id="6f190-115">Int64</span></span>  | <span data-ttu-id="6f190-116">Количество файлов, которые были просмотрены, изменены, предоставлены в общий доступ или синхронизированы в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="6f190-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="6f190-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="6f190-117">reportDate</span></span>        | <span data-ttu-id="6f190-118">Дата</span><span class="sxs-lookup"><span data-stu-id="6f190-118">Date</span></span>   | <span data-ttu-id="6f190-119">Дата, когда число файлов было активно на сайте SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="6f190-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="6f190-120">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="6f190-120">reportPeriod</span></span>      | <span data-ttu-id="6f190-121">String</span><span class="sxs-lookup"><span data-stu-id="6f190-121">String</span></span> | <span data-ttu-id="6f190-122">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="6f190-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6f190-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f190-123">JSON representation</span></span>

<span data-ttu-id="6f190-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f190-124">The following is a JSON representation of the resource.</span></span>

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
