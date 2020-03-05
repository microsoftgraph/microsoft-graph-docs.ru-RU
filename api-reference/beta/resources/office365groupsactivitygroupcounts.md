---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: bf84a0dcd2fc542735398e0aec2c6eb710d3f2f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522437"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="82c38-103">Тип ресурса office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="82c38-103">office365GroupsActivityGroupCounts resource type</span></span>

<span data-ttu-id="82c38-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="82c38-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="82c38-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="82c38-105">Properties</span></span>

| <span data-ttu-id="82c38-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="82c38-106">Property</span></span>          | <span data-ttu-id="82c38-107">Тип</span><span class="sxs-lookup"><span data-stu-id="82c38-107">Type</span></span>   | <span data-ttu-id="82c38-108">Описание</span><span class="sxs-lookup"><span data-stu-id="82c38-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="82c38-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="82c38-109">reportRefreshDate</span></span> | <span data-ttu-id="82c38-110">Дата</span><span class="sxs-lookup"><span data-stu-id="82c38-110">Date</span></span>   | <span data-ttu-id="82c38-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="82c38-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="82c38-112">total</span><span class="sxs-lookup"><span data-stu-id="82c38-112">total</span></span>             | <span data-ttu-id="82c38-113">Int64</span><span class="sxs-lookup"><span data-stu-id="82c38-113">Int64</span></span>  | <span data-ttu-id="82c38-114">Общее количество групп.</span><span class="sxs-lookup"><span data-stu-id="82c38-114">The total number of groups.</span></span>              |
| <span data-ttu-id="82c38-115">ASP</span><span class="sxs-lookup"><span data-stu-id="82c38-115">active</span></span>            | <span data-ttu-id="82c38-116">Int64</span><span class="sxs-lookup"><span data-stu-id="82c38-116">Int64</span></span>  | <span data-ttu-id="82c38-117">Количество активных групп.</span><span class="sxs-lookup"><span data-stu-id="82c38-117">The number of active groups.</span></span> <span data-ttu-id="82c38-118">Группа считается активной при возникновении любой из следующих условий: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="82c38-118">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="82c38-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="82c38-119">reportDate</span></span>        | <span data-ttu-id="82c38-120">Дата</span><span class="sxs-lookup"><span data-stu-id="82c38-120">Date</span></span>   | <span data-ttu-id="82c38-121">Дата активности ряда групп.</span><span class="sxs-lookup"><span data-stu-id="82c38-121">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="82c38-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="82c38-122">reportPeriod</span></span>      | <span data-ttu-id="82c38-123">String</span><span class="sxs-lookup"><span data-stu-id="82c38-123">String</span></span> | <span data-ttu-id="82c38-124">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="82c38-124">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="82c38-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="82c38-125">JSON representation</span></span>

<span data-ttu-id="82c38-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82c38-126">The following is a JSON representation of the resource.</span></span>

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
