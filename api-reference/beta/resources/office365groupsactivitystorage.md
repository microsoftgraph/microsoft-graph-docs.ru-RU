---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 180e60a52b397f969aa10cee5bc27bba934ad1e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944455"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="ebc09-103">Тип ресурса office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="ebc09-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ebc09-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebc09-104">Properties</span></span>

| <span data-ttu-id="ebc09-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebc09-105">Property</span></span>                  | <span data-ttu-id="ebc09-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ebc09-106">Type</span></span>   | <span data-ttu-id="ebc09-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc09-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="ebc09-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ebc09-108">reportRefreshDate</span></span>         | <span data-ttu-id="ebc09-109">Date</span><span class="sxs-lookup"><span data-stu-id="ebc09-109">Date</span></span>   | <span data-ttu-id="ebc09-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="ebc09-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ebc09-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ebc09-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="ebc09-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ebc09-112">Int64</span></span>  | <span data-ttu-id="ebc09-113">Используются в почтовом ящике группы хранения.</span><span class="sxs-lookup"><span data-stu-id="ebc09-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="ebc09-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ebc09-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="ebc09-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ebc09-115">Int64</span></span>  | <span data-ttu-id="ebc09-116">Хранения, используемый в библиотеке документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ebc09-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="ebc09-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="ebc09-117">reportDate</span></span>                | <span data-ttu-id="ebc09-118">Date</span><span class="sxs-lookup"><span data-stu-id="ebc09-118">Date</span></span>   | <span data-ttu-id="ebc09-119">Дата моментальный снимок для Exchange и SharePoint используется хранилища.</span><span class="sxs-lookup"><span data-stu-id="ebc09-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="ebc09-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ebc09-120">reportPeriod</span></span>              | <span data-ttu-id="ebc09-121">Строка</span><span class="sxs-lookup"><span data-stu-id="ebc09-121">String</span></span> | <span data-ttu-id="ebc09-122">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="ebc09-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ebc09-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebc09-123">JSON representation</span></span>

<span data-ttu-id="ebc09-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebc09-124">The following is a JSON representation of the resource.</span></span>

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
