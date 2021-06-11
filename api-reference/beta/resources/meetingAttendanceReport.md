---
title: тип ресурса meetingAttendanceReport
description: Содержит сведения, связанные с отчетом о посещаемости собрания.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f1ea75f6e57d0e095a470e715e080c7def05ab46
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896727"
---
# <a name="meetingattendancereport-resource-type"></a><span data-ttu-id="a7a17-103">тип ресурса meetingAttendanceReport</span><span class="sxs-lookup"><span data-stu-id="a7a17-103">meetingAttendanceReport resource type</span></span>

<span data-ttu-id="a7a17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7a17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7a17-105">Содержит сведения, связанные с отчетом о посещаемости собрания.</span><span class="sxs-lookup"><span data-stu-id="a7a17-105">Contains information associated with meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="a7a17-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7a17-106">Properties</span></span>

| <span data-ttu-id="a7a17-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7a17-107">Property</span></span>            | <span data-ttu-id="a7a17-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a7a17-108">Type</span></span>    | <span data-ttu-id="a7a17-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a7a17-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="a7a17-110">attendanceRecords</span><span class="sxs-lookup"><span data-stu-id="a7a17-110">attendanceRecords</span></span>           | <span data-ttu-id="a7a17-111">[коллекция attendanceRecord](attendanceRecord.md)</span><span class="sxs-lookup"><span data-stu-id="a7a17-111">[attendanceRecord](attendanceRecord.md) collection</span></span>  | <span data-ttu-id="a7a17-112">Список записей о посещаемости.</span><span class="sxs-lookup"><span data-stu-id="a7a17-112">The list of attendance records.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a7a17-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7a17-113">JSON representation</span></span>

<span data-ttu-id="a7a17-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7a17-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```json
{
  "attendanceRecords": [{"@odata.type": "#microsoft.graph.attendanceRecord"}]
}
```
