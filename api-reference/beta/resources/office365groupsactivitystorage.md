---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac9ca260e4723f7c4aeca8e15f837d4cd57b7c4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982182"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="3e5c5-103">Тип ресурса office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="3e5c5-103">office365GroupsActivityStorage resource type</span></span>

<span data-ttu-id="3e5c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e5c5-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3e5c5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e5c5-105">Properties</span></span>

| <span data-ttu-id="3e5c5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e5c5-106">Property</span></span>                  | <span data-ttu-id="3e5c5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3e5c5-107">Type</span></span>   | <span data-ttu-id="3e5c5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3e5c5-108">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="3e5c5-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3e5c5-109">reportRefreshDate</span></span>         | <span data-ttu-id="3e5c5-110">Дата</span><span class="sxs-lookup"><span data-stu-id="3e5c5-110">Date</span></span>   | <span data-ttu-id="3e5c5-111">Последняя дата содержимого.</span><span class="sxs-lookup"><span data-stu-id="3e5c5-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="3e5c5-112">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="3e5c5-112">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="3e5c5-113">Int64</span><span class="sxs-lookup"><span data-stu-id="3e5c5-113">Int64</span></span>  | <span data-ttu-id="3e5c5-114">Хранилище, используемого в почтовом ящике группы.</span><span class="sxs-lookup"><span data-stu-id="3e5c5-114">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="3e5c5-115">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="3e5c5-115">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="3e5c5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3e5c5-116">Int64</span></span>  | <span data-ttu-id="3e5c5-117">Хранилище, используемого в библиотеке документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3e5c5-117">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="3e5c5-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="3e5c5-118">reportDate</span></span>                | <span data-ttu-id="3e5c5-119">Дата</span><span class="sxs-lookup"><span data-stu-id="3e5c5-119">Date</span></span>   | <span data-ttu-id="3e5c5-120">Моментальный снимок используемого хранилища Exchange и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3e5c5-120">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="3e5c5-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3e5c5-121">reportPeriod</span></span>              | <span data-ttu-id="3e5c5-122">String</span><span class="sxs-lookup"><span data-stu-id="3e5c5-122">String</span></span> | <span data-ttu-id="3e5c5-123">Количество дней в отчете.</span><span class="sxs-lookup"><span data-stu-id="3e5c5-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="3e5c5-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e5c5-124">JSON representation</span></span>

<span data-ttu-id="3e5c5-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e5c5-125">The following is a JSON representation of the resource.</span></span>

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


