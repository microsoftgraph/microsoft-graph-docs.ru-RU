---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0b14e6981a193ad1698303d2762d0321de430b73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092393"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="398f7-103">Тип ресурса office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="398f7-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="398f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="398f7-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="398f7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="398f7-105">Properties</span></span>

| <span data-ttu-id="398f7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="398f7-106">Property</span></span>                  | <span data-ttu-id="398f7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="398f7-107">Type</span></span>   | <span data-ttu-id="398f7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="398f7-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="398f7-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="398f7-109">reportRefreshDate</span></span>         | <span data-ttu-id="398f7-110">Дата</span><span class="sxs-lookup"><span data-stu-id="398f7-110">Date</span></span>   | <span data-ttu-id="398f7-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="398f7-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="398f7-112">маилбокссторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="398f7-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="398f7-113">Int64</span><span class="sxs-lookup"><span data-stu-id="398f7-113">Int64</span></span>  | <span data-ttu-id="398f7-114">Хранилище, используемое в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="398f7-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="398f7-115">ситесторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="398f7-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="398f7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="398f7-116">Int64</span></span>  | <span data-ttu-id="398f7-117">Хранилище, используемое в библиотеке документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="398f7-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="398f7-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="398f7-118">reportDate</span></span>                | <span data-ttu-id="398f7-119">Дата</span><span class="sxs-lookup"><span data-stu-id="398f7-119">Date</span></span>   | <span data-ttu-id="398f7-120">Дата моментального снимка хранилища для Exchange и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="398f7-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="398f7-121">репортпериод</span><span class="sxs-lookup"><span data-stu-id="398f7-121">reportPeriod</span></span>              | <span data-ttu-id="398f7-122">Строка</span><span class="sxs-lookup"><span data-stu-id="398f7-122">String</span></span> | <span data-ttu-id="398f7-123">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="398f7-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="398f7-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="398f7-124">JSON representation</span></span>

<span data-ttu-id="398f7-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="398f7-125">The following is a JSON representation of the resource.</span></span>

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


