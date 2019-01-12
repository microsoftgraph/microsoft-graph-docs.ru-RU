---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d3c1272f9bd99c3e7ee0f29a4c303e1c8ca95525
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975885"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="2e03c-103">Тип ресурса office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="2e03c-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2e03c-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e03c-104">Properties</span></span>

| <span data-ttu-id="2e03c-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e03c-105">Property</span></span>          | <span data-ttu-id="2e03c-106">Тип</span><span class="sxs-lookup"><span data-stu-id="2e03c-106">Type</span></span>   | <span data-ttu-id="2e03c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2e03c-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2e03c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2e03c-108">reportRefreshDate</span></span> | <span data-ttu-id="2e03c-109">Date</span><span class="sxs-lookup"><span data-stu-id="2e03c-109">Date</span></span>   | <span data-ttu-id="2e03c-110">Последняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="2e03c-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2e03c-111">total</span><span class="sxs-lookup"><span data-stu-id="2e03c-111">total</span></span>             | <span data-ttu-id="2e03c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2e03c-112">Int64</span></span>  | <span data-ttu-id="2e03c-113">Общее число групп.</span><span class="sxs-lookup"><span data-stu-id="2e03c-113">The total number of groups.</span></span>              |
| <span data-ttu-id="2e03c-114">активных</span><span class="sxs-lookup"><span data-stu-id="2e03c-114">active</span></span>            | <span data-ttu-id="2e03c-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2e03c-115">Int64</span></span>  | <span data-ttu-id="2e03c-116">Число активных групп.</span><span class="sxs-lookup"><span data-stu-id="2e03c-116">The number of active groups.</span></span> <span data-ttu-id="2e03c-117">Группы считается активным, если какие-либо из следующих значений: групповой полученных почтового ящика электронной почты; пользователю просматривать, редактировать, общих или синхронизирован файлы в библиотеке документов SharePoint. пользователь просматривает страницы SharePoint; пользователь учтена, чтение или оцененных сообщений в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="2e03c-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="2e03c-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="2e03c-118">reportDate</span></span>        | <span data-ttu-id="2e03c-119">Date</span><span class="sxs-lookup"><span data-stu-id="2e03c-119">Date</span></span>   | <span data-ttu-id="2e03c-120">Дата, на котором выполнялись число групп.</span><span class="sxs-lookup"><span data-stu-id="2e03c-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="2e03c-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2e03c-121">reportPeriod</span></span>      | <span data-ttu-id="2e03c-122">Строка</span><span class="sxs-lookup"><span data-stu-id="2e03c-122">String</span></span> | <span data-ttu-id="2e03c-123">Количество дней, на которое отчета.</span><span class="sxs-lookup"><span data-stu-id="2e03c-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2e03c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e03c-124">JSON representation</span></span>

<span data-ttu-id="2e03c-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e03c-125">The following is a JSON representation of the resource.</span></span>

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
