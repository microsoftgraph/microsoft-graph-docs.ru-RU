---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b202d5189c1edeeeaa45d447aa7cc078dd263858
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581424"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a><span data-ttu-id="c263d-103">Тип ресурса office365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="c263d-103">office365GroupsActivityGroupCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c263d-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="c263d-104">Properties</span></span>

| <span data-ttu-id="c263d-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c263d-105">Property</span></span>          | <span data-ttu-id="c263d-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c263d-106">Type</span></span>   | <span data-ttu-id="c263d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c263d-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="c263d-108">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="c263d-108">reportRefreshDate</span></span> | <span data-ttu-id="c263d-109">Дата</span><span class="sxs-lookup"><span data-stu-id="c263d-109">Date</span></span>   | <span data-ttu-id="c263d-110">Самая поздняя дата контента.</span><span class="sxs-lookup"><span data-stu-id="c263d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="c263d-111">total</span><span class="sxs-lookup"><span data-stu-id="c263d-111">total</span></span>             | <span data-ttu-id="c263d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c263d-112">Int64</span></span>  | <span data-ttu-id="c263d-113">Общее количество групп.</span><span class="sxs-lookup"><span data-stu-id="c263d-113">The total number of groups.</span></span>              |
| <span data-ttu-id="c263d-114">ASP</span><span class="sxs-lookup"><span data-stu-id="c263d-114">active</span></span>            | <span data-ttu-id="c263d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c263d-115">Int64</span></span>  | <span data-ttu-id="c263d-116">Количество активных групп.</span><span class="sxs-lookup"><span data-stu-id="c263d-116">The number of active groups.</span></span> <span data-ttu-id="c263d-117">Группа считается активной при возникновении любой из следующих условий: группового почтового ящика получено сообщение электронной почты; Пользователи, которые просматривали, редактирующие, совместно используемые или синхронизированные файлы в библиотеке документов SharePoint; страницы SharePoint, просмотренные пользователями; Разнесенные, прочитанные или понравившиеся сообщения пользователя в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="c263d-117">A group is considered active if any of the following occurred: group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="c263d-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="c263d-118">reportDate</span></span>        | <span data-ttu-id="c263d-119">Дата</span><span class="sxs-lookup"><span data-stu-id="c263d-119">Date</span></span>   | <span data-ttu-id="c263d-120">Дата активности ряда групп.</span><span class="sxs-lookup"><span data-stu-id="c263d-120">The date on which a number of groups were active.</span></span> |
| <span data-ttu-id="c263d-121">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="c263d-121">reportPeriod</span></span>      | <span data-ttu-id="c263d-122">String</span><span class="sxs-lookup"><span data-stu-id="c263d-122">String</span></span> | <span data-ttu-id="c263d-123">Количество дней, охватываемых отчетом.</span><span class="sxs-lookup"><span data-stu-id="c263d-123">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c263d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c263d-124">JSON representation</span></span>

<span data-ttu-id="c263d-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c263d-125">The following is a JSON representation of the resource.</span></span>

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
