---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adff009d9047aa147c8042059fbdab8491288fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972560"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="d9a2b-103">Тип ресурса office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="d9a2b-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d9a2b-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9a2b-104">Properties</span></span>

| <span data-ttu-id="d9a2b-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9a2b-105">Property</span></span>          | <span data-ttu-id="d9a2b-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d9a2b-106">Type</span></span>   | <span data-ttu-id="d9a2b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d9a2b-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d9a2b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d9a2b-108">reportRefreshDate</span></span> | <span data-ttu-id="d9a2b-109">Date</span><span class="sxs-lookup"><span data-stu-id="d9a2b-109">Date</span></span>   | <span data-ttu-id="d9a2b-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="d9a2b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d9a2b-111">total</span><span class="sxs-lookup"><span data-stu-id="d9a2b-111">total</span></span>             | <span data-ttu-id="d9a2b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d9a2b-112">Int64</span></span>  | <span data-ttu-id="d9a2b-113">Общее число файлов в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="d9a2b-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="d9a2b-114">активных</span><span class="sxs-lookup"><span data-stu-id="d9a2b-114">active</span></span>            | <span data-ttu-id="d9a2b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d9a2b-115">Int64</span></span>  | <span data-ttu-id="d9a2b-116">Число файлов, которые были просматривать, редактировать, общих или синхронизирован в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="d9a2b-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="d9a2b-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="d9a2b-117">reportDate</span></span>        | <span data-ttu-id="d9a2b-118">Date</span><span class="sxs-lookup"><span data-stu-id="d9a2b-118">Date</span></span>   | <span data-ttu-id="d9a2b-119">Дата, на котором количество файлов были активны на сайте группы SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d9a2b-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="d9a2b-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d9a2b-120">reportPeriod</span></span>      | <span data-ttu-id="d9a2b-121">Строка</span><span class="sxs-lookup"><span data-stu-id="d9a2b-121">String</span></span> | <span data-ttu-id="d9a2b-122">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="d9a2b-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d9a2b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9a2b-123">JSON representation</span></span>

<span data-ttu-id="d9a2b-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9a2b-124">The following is a JSON representation of the resource.</span></span>

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
