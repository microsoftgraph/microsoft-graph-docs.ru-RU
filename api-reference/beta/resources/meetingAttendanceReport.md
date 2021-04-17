---
title: тип ресурса meetingAttendanceReport
description: Содержит сведения, связанные с отчетом о посещаемости собрания.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 011250c97ae660937a1bad8e008e4932bb5fb289
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882719"
---
# <a name="meetingattendancereport-resource-type"></a><span data-ttu-id="4e80b-103">тип ресурса meetingAttendanceReport</span><span class="sxs-lookup"><span data-stu-id="4e80b-103">meetingAttendanceReport resource type</span></span>

<span data-ttu-id="4e80b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e80b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e80b-105">Содержит сведения, связанные с отчетом о посещаемости собрания.</span><span class="sxs-lookup"><span data-stu-id="4e80b-105">Contains information associated with meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="4e80b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e80b-106">Properties</span></span>

| <span data-ttu-id="4e80b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e80b-107">Property</span></span>            | <span data-ttu-id="4e80b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4e80b-108">Type</span></span>    | <span data-ttu-id="4e80b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e80b-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="4e80b-110">attendanceRecords</span><span class="sxs-lookup"><span data-stu-id="4e80b-110">attendanceRecords</span></span>           | <span data-ttu-id="4e80b-111">[коллекция attendanceRecord](attendanceRecord.md)</span><span class="sxs-lookup"><span data-stu-id="4e80b-111">[attendanceRecord](attendanceRecord.md) collection</span></span>  | <span data-ttu-id="4e80b-112">Список записей о посещаемости.</span><span class="sxs-lookup"><span data-stu-id="4e80b-112">The list of attendance records.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4e80b-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e80b-113">JSON representation</span></span>

<span data-ttu-id="4e80b-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e80b-114">The following is a JSON representation of the resource.</span></span>

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
