---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505552"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="e55d5-103">Тип ресурса office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="e55d5-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e55d5-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e55d5-104">Properties</span></span>

| <span data-ttu-id="e55d5-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e55d5-105">Property</span></span>                  | <span data-ttu-id="e55d5-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e55d5-106">Type</span></span>   | <span data-ttu-id="e55d5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e55d5-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="e55d5-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="e55d5-108">reportRefreshDate</span></span>         | <span data-ttu-id="e55d5-109">Дата</span><span class="sxs-lookup"><span data-stu-id="e55d5-109">Date</span></span>   | <span data-ttu-id="e55d5-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="e55d5-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="e55d5-111">Маилбокссторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="e55d5-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="e55d5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e55d5-112">Int64</span></span>  | <span data-ttu-id="e55d5-113">Хранилище, используемое в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="e55d5-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="e55d5-114">Ситесторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="e55d5-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="e55d5-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e55d5-115">Int64</span></span>  | <span data-ttu-id="e55d5-116">Хранилище, используемое в библиотеке документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e55d5-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="e55d5-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="e55d5-117">reportDate</span></span>                | <span data-ttu-id="e55d5-118">Дата</span><span class="sxs-lookup"><span data-stu-id="e55d5-118">Date</span></span>   | <span data-ttu-id="e55d5-119">Дата моментального снимка хранилища для Exchange и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e55d5-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="e55d5-120">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="e55d5-120">reportPeriod</span></span>              | <span data-ttu-id="e55d5-121">String</span><span class="sxs-lookup"><span data-stu-id="e55d5-121">String</span></span> | <span data-ttu-id="e55d5-122">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="e55d5-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="e55d5-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e55d5-123">JSON representation</span></span>

<span data-ttu-id="e55d5-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e55d5-124">The following is a JSON representation of the resource.</span></span>

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
