---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: ed5386083b11fb6fe7f063a4890744532feeb081
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832622"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="7d1f4-103">Тип ресурса office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="7d1f4-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7d1f4-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d1f4-104">Properties</span></span>

| <span data-ttu-id="7d1f4-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d1f4-105">Property</span></span>          | <span data-ttu-id="7d1f4-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7d1f4-106">Type</span></span>   | <span data-ttu-id="7d1f4-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7d1f4-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="7d1f4-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7d1f4-108">reportRefreshDate</span></span> | <span data-ttu-id="7d1f4-109">Date</span><span class="sxs-lookup"><span data-stu-id="7d1f4-109">Date</span></span>   | <span data-ttu-id="7d1f4-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="7d1f4-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="7d1f4-111">total</span><span class="sxs-lookup"><span data-stu-id="7d1f4-111">total</span></span>             | <span data-ttu-id="7d1f4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7d1f4-112">Int64</span></span>  | <span data-ttu-id="7d1f4-113">Общее число групп.</span><span class="sxs-lookup"><span data-stu-id="7d1f4-113">The total number of groups.</span></span>              |
| <span data-ttu-id="7d1f4-114">активных</span><span class="sxs-lookup"><span data-stu-id="7d1f4-114">active</span></span>            | <span data-ttu-id="7d1f4-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7d1f4-115">Int64</span></span>  | <span data-ttu-id="7d1f4-116">Число активных групп.</span><span class="sxs-lookup"><span data-stu-id="7d1f4-116">The number of active groups.</span></span> <span data-ttu-id="7d1f4-117">Группы считается активным, если какие-либо из следующих значений: групповой полученных почтового ящика электронной почты; пользователю просматривать, редактировать, общих или синхронизирован файлы в библиотеке документов SharePoint. пользователь просматривает страницы SharePoint; пользователь учтена, чтение или оцененных сообщений в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="7d1f4-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="7d1f4-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="7d1f4-118">reportDate</span></span>        | <span data-ttu-id="7d1f4-119">Date</span><span class="sxs-lookup"><span data-stu-id="7d1f4-119">Date</span></span>   | <span data-ttu-id="7d1f4-120">Дата, на котором выполнялись число групп.</span><span class="sxs-lookup"><span data-stu-id="7d1f4-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="7d1f4-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7d1f4-121">reportPeriod</span></span>      | <span data-ttu-id="7d1f4-122">Строка</span><span class="sxs-lookup"><span data-stu-id="7d1f4-122">String</span></span> | <span data-ttu-id="7d1f4-123">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="7d1f4-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="7d1f4-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d1f4-124">JSON representation</span></span>

<span data-ttu-id="7d1f4-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d1f4-125">The following is a JSON representation of the resource.</span></span>

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
