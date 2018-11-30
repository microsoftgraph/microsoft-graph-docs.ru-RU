---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 23ff4d112373f52c4c19d6631ac89bac22399b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081592"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="56225-103">Тип ресурса office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="56225-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="56225-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="56225-104">Properties</span></span>

| <span data-ttu-id="56225-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="56225-105">Property</span></span>                  | <span data-ttu-id="56225-106">Тип</span><span class="sxs-lookup"><span data-stu-id="56225-106">Type</span></span>   | <span data-ttu-id="56225-107">Description</span><span class="sxs-lookup"><span data-stu-id="56225-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="56225-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="56225-108">reportRefreshDate</span></span>         | <span data-ttu-id="56225-109">Date</span><span class="sxs-lookup"><span data-stu-id="56225-109">Date</span></span>   | <span data-ttu-id="56225-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="56225-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="56225-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="56225-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="56225-112">Int64</span><span class="sxs-lookup"><span data-stu-id="56225-112">Int64</span></span>  | <span data-ttu-id="56225-113">Используются в почтовом ящике группы хранения.</span><span class="sxs-lookup"><span data-stu-id="56225-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="56225-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="56225-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="56225-115">Int64</span><span class="sxs-lookup"><span data-stu-id="56225-115">Int64</span></span>  | <span data-ttu-id="56225-116">Хранения, используемый в библиотеке документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="56225-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="56225-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="56225-117">reportDate</span></span>                | <span data-ttu-id="56225-118">Date</span><span class="sxs-lookup"><span data-stu-id="56225-118">Date</span></span>   | <span data-ttu-id="56225-119">Дата моментальный снимок для Exchange и SharePoint используется хранилища.</span><span class="sxs-lookup"><span data-stu-id="56225-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="56225-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="56225-120">reportPeriod</span></span>              | <span data-ttu-id="56225-121">String</span><span class="sxs-lookup"><span data-stu-id="56225-121">String</span></span> | <span data-ttu-id="56225-122">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="56225-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="56225-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56225-123">JSON representation</span></span>

<span data-ttu-id="56225-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56225-124">The following is a JSON representation of the resource.</span></span>

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
