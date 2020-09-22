---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c249123a01cde2fe952f5111affe645415ddc6cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092386"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="359d5-103">Тип ресурса office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="359d5-103">office365GroupsActivityGroupCounts resource type</span></span>

<span data-ttu-id="359d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="359d5-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="359d5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="359d5-105">Properties</span></span>

| <span data-ttu-id="359d5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="359d5-106">Property</span></span>          | <span data-ttu-id="359d5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="359d5-107">Type</span></span>   | <span data-ttu-id="359d5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="359d5-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="359d5-109">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="359d5-109">reportRefreshDate</span></span> | <span data-ttu-id="359d5-110">Дата</span><span class="sxs-lookup"><span data-stu-id="359d5-110">Date</span></span>   | <span data-ttu-id="359d5-111">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="359d5-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="359d5-112">total</span><span class="sxs-lookup"><span data-stu-id="359d5-112">total</span></span>             | <span data-ttu-id="359d5-113">Int64</span><span class="sxs-lookup"><span data-stu-id="359d5-113">Int64</span></span>  | <span data-ttu-id="359d5-114">Общее количество групп.</span><span class="sxs-lookup"><span data-stu-id="359d5-114">The total number of groups.</span></span>              |
| <span data-ttu-id="359d5-115">ASP</span><span class="sxs-lookup"><span data-stu-id="359d5-115">active</span></span>            | <span data-ttu-id="359d5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="359d5-116">Int64</span></span>  | <span data-ttu-id="359d5-117">Количество активных групп.</span><span class="sxs-lookup"><span data-stu-id="359d5-117">The number of active groups.</span></span> <span data-ttu-id="359d5-118">Группа считается активной при возникновении любой из следующих условий: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="359d5-118">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="359d5-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="359d5-119">reportDate</span></span>        | <span data-ttu-id="359d5-120">Дата</span><span class="sxs-lookup"><span data-stu-id="359d5-120">Date</span></span>   | <span data-ttu-id="359d5-121">Дата активности ряда групп.</span><span class="sxs-lookup"><span data-stu-id="359d5-121">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="359d5-122">репортпериод</span><span class="sxs-lookup"><span data-stu-id="359d5-122">reportPeriod</span></span>      | <span data-ttu-id="359d5-123">Строка</span><span class="sxs-lookup"><span data-stu-id="359d5-123">String</span></span> | <span data-ttu-id="359d5-124">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="359d5-124">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="359d5-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="359d5-125">JSON representation</span></span>

<span data-ttu-id="359d5-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="359d5-126">The following is a JSON representation of the resource.</span></span>

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


