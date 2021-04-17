---
title: тип ресурса attendanceInterval
description: Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1746adc802534f72aa9d139c6a16d8da62dd9fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882725"
---
# <a name="attendanceinterval-resource-type"></a><span data-ttu-id="d3db7-103">тип ресурса attendanceInterval</span><span class="sxs-lookup"><span data-stu-id="d3db7-103">attendanceInterval resource type</span></span>

<span data-ttu-id="d3db7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3db7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3db7-105">Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.</span><span class="sxs-lookup"><span data-stu-id="d3db7-105">Contains information associated with attendance interval in attendanceRecord.</span></span>

## <a name="properties"></a><span data-ttu-id="d3db7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3db7-106">Properties</span></span>

| <span data-ttu-id="d3db7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3db7-107">Property</span></span>            | <span data-ttu-id="d3db7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d3db7-108">Type</span></span>    | <span data-ttu-id="d3db7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d3db7-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="d3db7-110">joinDateTime</span><span class="sxs-lookup"><span data-stu-id="d3db7-110">joinDateTime</span></span> | <span data-ttu-id="d3db7-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="d3db7-111">DateTime</span></span> | <span data-ttu-id="d3db7-112">Участник time присоединился к UTC.</span><span class="sxs-lookup"><span data-stu-id="d3db7-112">Time attendee joined in UTC.</span></span> |
| <span data-ttu-id="d3db7-113">leaveDateTime</span><span class="sxs-lookup"><span data-stu-id="d3db7-113">leaveDateTime</span></span> | <span data-ttu-id="d3db7-114">DateTime</span><span class="sxs-lookup"><span data-stu-id="d3db7-114">DateTime</span></span> | <span data-ttu-id="d3db7-115">Время участника, оставленного в UTC.</span><span class="sxs-lookup"><span data-stu-id="d3db7-115">Time attendee left in UTC.</span></span> |
| <span data-ttu-id="d3db7-116">durationInSeconds</span><span class="sxs-lookup"><span data-stu-id="d3db7-116">durationInSeconds</span></span> | <span data-ttu-id="d3db7-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d3db7-117">Int32</span></span> | <span data-ttu-id="d3db7-118">Продолжительность интервала собрания в секундах; то есть разница между **joinDateTime** и **leaveDateTime.**</span><span class="sxs-lookup"><span data-stu-id="d3db7-118">Duration of the meeting interval in seconds; that is, the difference between **joinDateTime** and **leaveDateTime**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d3db7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3db7-119">JSON representation</span></span>

<span data-ttu-id="d3db7-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3db7-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceInterval"
}-->

```json

{
    "joinDateTime": "String (timestamp)",
    "leaveDateTime": "String (timestamp)",
    "durationInSeconds": "Int32"
}
    
```
