---
title: тип ресурса attendanceInterval
description: Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13b4e20a5233b865dd5417eed4d159bce07c8717
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896517"
---
# <a name="attendanceinterval-resource-type"></a><span data-ttu-id="1cb85-103">тип ресурса attendanceInterval</span><span class="sxs-lookup"><span data-stu-id="1cb85-103">attendanceInterval resource type</span></span>

<span data-ttu-id="1cb85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cb85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cb85-105">Содержит сведения, связанные с интервалом посещаемости в attendanceRecord.</span><span class="sxs-lookup"><span data-stu-id="1cb85-105">Contains information associated with attendance interval in attendanceRecord.</span></span>

## <a name="properties"></a><span data-ttu-id="1cb85-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cb85-106">Properties</span></span>

| <span data-ttu-id="1cb85-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cb85-107">Property</span></span>            | <span data-ttu-id="1cb85-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1cb85-108">Type</span></span>    | <span data-ttu-id="1cb85-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb85-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="1cb85-110">joinDateTime</span><span class="sxs-lookup"><span data-stu-id="1cb85-110">joinDateTime</span></span> | <span data-ttu-id="1cb85-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="1cb85-111">DateTime</span></span> | <span data-ttu-id="1cb85-112">Участник time присоединился к UTC.</span><span class="sxs-lookup"><span data-stu-id="1cb85-112">Time attendee joined in UTC.</span></span> |
| <span data-ttu-id="1cb85-113">leaveDateTime</span><span class="sxs-lookup"><span data-stu-id="1cb85-113">leaveDateTime</span></span> | <span data-ttu-id="1cb85-114">DateTime</span><span class="sxs-lookup"><span data-stu-id="1cb85-114">DateTime</span></span> | <span data-ttu-id="1cb85-115">Время участника, оставленного в UTC.</span><span class="sxs-lookup"><span data-stu-id="1cb85-115">Time attendee left in UTC.</span></span> |
| <span data-ttu-id="1cb85-116">durationInSeconds</span><span class="sxs-lookup"><span data-stu-id="1cb85-116">durationInSeconds</span></span> | <span data-ttu-id="1cb85-117">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb85-117">Int32</span></span> | <span data-ttu-id="1cb85-118">Продолжительность интервала собрания в секундах; то есть разница между **joinDateTime** и **leaveDateTime.**</span><span class="sxs-lookup"><span data-stu-id="1cb85-118">Duration of the meeting interval in seconds; that is, the difference between **joinDateTime** and **leaveDateTime**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1cb85-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1cb85-119">JSON representation</span></span>

<span data-ttu-id="1cb85-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cb85-120">The following is a JSON representation of the resource.</span></span>

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
