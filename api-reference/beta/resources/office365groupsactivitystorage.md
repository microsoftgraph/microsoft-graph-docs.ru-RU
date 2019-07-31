---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: a3168ad417f246017ba1018aca265ec0363c951e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009463"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="fe3b2-103">Тип ресурса office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="fe3b2-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fe3b2-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe3b2-104">Properties</span></span>

| <span data-ttu-id="fe3b2-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe3b2-105">Property</span></span>                  | <span data-ttu-id="fe3b2-106">Тип</span><span class="sxs-lookup"><span data-stu-id="fe3b2-106">Type</span></span>   | <span data-ttu-id="fe3b2-107">Описание</span><span class="sxs-lookup"><span data-stu-id="fe3b2-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="fe3b2-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="fe3b2-108">reportRefreshDate</span></span>         | <span data-ttu-id="fe3b2-109">Дата</span><span class="sxs-lookup"><span data-stu-id="fe3b2-109">Date</span></span>   | <span data-ttu-id="fe3b2-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="fe3b2-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="fe3b2-111">Маилбокссторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="fe3b2-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="fe3b2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fe3b2-112">Int64</span></span>  | <span data-ttu-id="fe3b2-113">Хранилище, используемое в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="fe3b2-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="fe3b2-114">Ситесторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="fe3b2-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="fe3b2-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fe3b2-115">Int64</span></span>  | <span data-ttu-id="fe3b2-116">Хранилище, используемое в библиотеке документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fe3b2-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="fe3b2-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="fe3b2-117">reportDate</span></span>                | <span data-ttu-id="fe3b2-118">Дата</span><span class="sxs-lookup"><span data-stu-id="fe3b2-118">Date</span></span>   | <span data-ttu-id="fe3b2-119">Дата моментального снимка хранилища для Exchange и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fe3b2-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="fe3b2-120">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="fe3b2-120">reportPeriod</span></span>              | <span data-ttu-id="fe3b2-121">String</span><span class="sxs-lookup"><span data-stu-id="fe3b2-121">String</span></span> | <span data-ttu-id="fe3b2-122">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="fe3b2-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="fe3b2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe3b2-123">JSON representation</span></span>

<span data-ttu-id="fe3b2-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe3b2-124">The following is a JSON representation of the resource.</span></span>

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
