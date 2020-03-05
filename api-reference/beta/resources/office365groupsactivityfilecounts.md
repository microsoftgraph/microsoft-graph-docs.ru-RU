---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: dff3266aa268f2d26ca15492c72fa25a5f562a29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522444"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="9a684-103">Тип ресурса office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="9a684-103">office365GroupsActivityFileCounts resource type</span></span>

<span data-ttu-id="9a684-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9a684-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="9a684-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a684-105">Properties</span></span>

| <span data-ttu-id="9a684-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a684-106">Property</span></span>          | <span data-ttu-id="9a684-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9a684-107">Type</span></span>   | <span data-ttu-id="9a684-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9a684-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="9a684-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="9a684-109">reportRefreshDate</span></span> | <span data-ttu-id="9a684-110">Дата</span><span class="sxs-lookup"><span data-stu-id="9a684-110">Date</span></span>   | <span data-ttu-id="9a684-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="9a684-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="9a684-112">total</span><span class="sxs-lookup"><span data-stu-id="9a684-112">total</span></span>             | <span data-ttu-id="9a684-113">Int64</span><span class="sxs-lookup"><span data-stu-id="9a684-113">Int64</span></span>  | <span data-ttu-id="9a684-114">Общее количество файлов в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="9a684-114">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="9a684-115">ASP</span><span class="sxs-lookup"><span data-stu-id="9a684-115">active</span></span>            | <span data-ttu-id="9a684-116">Int64</span><span class="sxs-lookup"><span data-stu-id="9a684-116">Int64</span></span>  | <span data-ttu-id="9a684-117">Количество файлов, которые были просмотрены, изменены, предоставлены в общий доступ или синхронизированы в библиотеке документов SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="9a684-117">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="9a684-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="9a684-118">reportDate</span></span>        | <span data-ttu-id="9a684-119">Дата</span><span class="sxs-lookup"><span data-stu-id="9a684-119">Date</span></span>   | <span data-ttu-id="9a684-120">Дата, когда число файлов было активно на сайте SharePoint группы.</span><span class="sxs-lookup"><span data-stu-id="9a684-120">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="9a684-121">репортпериод</span><span class="sxs-lookup"><span data-stu-id="9a684-121">reportPeriod</span></span>      | <span data-ttu-id="9a684-122">String</span><span class="sxs-lookup"><span data-stu-id="9a684-122">String</span></span> | <span data-ttu-id="9a684-123">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="9a684-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="9a684-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a684-124">JSON representation</span></span>

<span data-ttu-id="9a684-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a684-125">The following is a JSON representation of the resource.</span></span>

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
