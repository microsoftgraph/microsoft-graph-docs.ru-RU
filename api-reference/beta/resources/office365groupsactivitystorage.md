---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576383"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="ad171-103">Тип ресурса office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="ad171-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ad171-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad171-104">Properties</span></span>

| <span data-ttu-id="ad171-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad171-105">Property</span></span>                  | <span data-ttu-id="ad171-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ad171-106">Type</span></span>   | <span data-ttu-id="ad171-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ad171-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="ad171-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ad171-108">reportRefreshDate</span></span>         | <span data-ttu-id="ad171-109">Date</span><span class="sxs-lookup"><span data-stu-id="ad171-109">Date</span></span>   | <span data-ttu-id="ad171-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="ad171-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ad171-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ad171-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="ad171-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ad171-112">Int64</span></span>  | <span data-ttu-id="ad171-113">Используются в почтовом ящике группы хранения.</span><span class="sxs-lookup"><span data-stu-id="ad171-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="ad171-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ad171-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="ad171-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ad171-115">Int64</span></span>  | <span data-ttu-id="ad171-116">Хранения, используемый в библиотеке документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ad171-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="ad171-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="ad171-117">reportDate</span></span>                | <span data-ttu-id="ad171-118">Date</span><span class="sxs-lookup"><span data-stu-id="ad171-118">Date</span></span>   | <span data-ttu-id="ad171-119">Дата моментальный снимок для Exchange и SharePoint используется хранилища.</span><span class="sxs-lookup"><span data-stu-id="ad171-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="ad171-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ad171-120">reportPeriod</span></span>              | <span data-ttu-id="ad171-121">Строка</span><span class="sxs-lookup"><span data-stu-id="ad171-121">String</span></span> | <span data-ttu-id="ad171-122">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="ad171-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ad171-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad171-123">JSON representation</span></span>

<span data-ttu-id="ad171-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad171-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
