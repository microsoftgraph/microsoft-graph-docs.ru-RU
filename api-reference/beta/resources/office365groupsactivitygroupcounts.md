---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b202d5189c1edeeeaa45d447aa7cc078dd263858
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572488"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="39a09-103">Тип ресурса office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="39a09-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="39a09-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="39a09-104">Properties</span></span>

| <span data-ttu-id="39a09-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="39a09-105">Property</span></span>          | <span data-ttu-id="39a09-106">Тип</span><span class="sxs-lookup"><span data-stu-id="39a09-106">Type</span></span>   | <span data-ttu-id="39a09-107">Описание</span><span class="sxs-lookup"><span data-stu-id="39a09-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="39a09-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="39a09-108">reportRefreshDate</span></span> | <span data-ttu-id="39a09-109">Date</span><span class="sxs-lookup"><span data-stu-id="39a09-109">Date</span></span>   | <span data-ttu-id="39a09-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="39a09-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="39a09-111">total</span><span class="sxs-lookup"><span data-stu-id="39a09-111">total</span></span>             | <span data-ttu-id="39a09-112">Int64</span><span class="sxs-lookup"><span data-stu-id="39a09-112">Int64</span></span>  | <span data-ttu-id="39a09-113">Общее число групп.</span><span class="sxs-lookup"><span data-stu-id="39a09-113">The total number of groups.</span></span>              |
| <span data-ttu-id="39a09-114">активных</span><span class="sxs-lookup"><span data-stu-id="39a09-114">active</span></span>            | <span data-ttu-id="39a09-115">Int64</span><span class="sxs-lookup"><span data-stu-id="39a09-115">Int64</span></span>  | <span data-ttu-id="39a09-116">Число активных групп.</span><span class="sxs-lookup"><span data-stu-id="39a09-116">The number of active groups.</span></span> <span data-ttu-id="39a09-117">Группы считается активным, если какие-либо из следующих значений: групповой полученных почтового ящика электронной почты; пользователю просматривать, редактировать, общих или синхронизирован файлы в библиотеке документов SharePoint. пользователь просматривает страницы SharePoint; пользователь учтена, чтение или оцененных сообщений в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="39a09-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="39a09-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="39a09-118">reportDate</span></span>        | <span data-ttu-id="39a09-119">Date</span><span class="sxs-lookup"><span data-stu-id="39a09-119">Date</span></span>   | <span data-ttu-id="39a09-120">Дата, на котором выполнялись число групп.</span><span class="sxs-lookup"><span data-stu-id="39a09-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="39a09-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="39a09-121">reportPeriod</span></span>      | <span data-ttu-id="39a09-122">Строка</span><span class="sxs-lookup"><span data-stu-id="39a09-122">String</span></span> | <span data-ttu-id="39a09-123">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="39a09-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="39a09-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39a09-124">JSON representation</span></span>

<span data-ttu-id="39a09-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39a09-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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
