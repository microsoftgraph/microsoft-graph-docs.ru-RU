---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: ba81621a819bb38f2d5d48e118729fc4476b5806
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522430"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="aca9f-103">Тип ресурса office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="aca9f-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="aca9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aca9f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="aca9f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="aca9f-105">Properties</span></span>

| <span data-ttu-id="aca9f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="aca9f-106">Property</span></span>                  | <span data-ttu-id="aca9f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="aca9f-107">Type</span></span>   | <span data-ttu-id="aca9f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="aca9f-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="aca9f-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="aca9f-109">reportRefreshDate</span></span>         | <span data-ttu-id="aca9f-110">Дата</span><span class="sxs-lookup"><span data-stu-id="aca9f-110">Date</span></span>   | <span data-ttu-id="aca9f-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="aca9f-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="aca9f-112">маилбокссторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="aca9f-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="aca9f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="aca9f-113">Int64</span></span>  | <span data-ttu-id="aca9f-114">Хранилище, используемое в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="aca9f-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="aca9f-115">ситесторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="aca9f-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="aca9f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="aca9f-116">Int64</span></span>  | <span data-ttu-id="aca9f-117">Хранилище, используемое в библиотеке документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="aca9f-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="aca9f-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="aca9f-118">reportDate</span></span>                | <span data-ttu-id="aca9f-119">Дата</span><span class="sxs-lookup"><span data-stu-id="aca9f-119">Date</span></span>   | <span data-ttu-id="aca9f-120">Дата моментального снимка хранилища для Exchange и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="aca9f-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="aca9f-121">репортпериод</span><span class="sxs-lookup"><span data-stu-id="aca9f-121">reportPeriod</span></span>              | <span data-ttu-id="aca9f-122">String</span><span class="sxs-lookup"><span data-stu-id="aca9f-122">String</span></span> | <span data-ttu-id="aca9f-123">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="aca9f-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="aca9f-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aca9f-124">JSON representation</span></span>

<span data-ttu-id="aca9f-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aca9f-125">The following is a JSON representation of the resource.</span></span>

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
