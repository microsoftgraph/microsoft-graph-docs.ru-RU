---
title: Тип ресурса метки времени
description: Дата и время сведения о времени.
localization_priority: Normal
ms.openlocfilehash: c63b3bba93f4b108a8eb9943d3fc2a1b2961f06c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888804"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="4c387-103">Тип ресурса метки времени</span><span class="sxs-lookup"><span data-stu-id="4c387-103">timeStamp resource type</span></span>

<span data-ttu-id="4c387-104">Дата и время сведения о времени.</span><span class="sxs-lookup"><span data-stu-id="4c387-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c387-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c387-105">JSON representation</span></span>

<span data-ttu-id="4c387-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4c387-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="4c387-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c387-107">Properties</span></span>
| <span data-ttu-id="4c387-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c387-108">Property</span></span>       | <span data-ttu-id="4c387-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4c387-109">Type</span></span>    |<span data-ttu-id="4c387-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4c387-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c387-111">date</span><span class="sxs-lookup"><span data-stu-id="4c387-111">date</span></span>|<span data-ttu-id="4c387-112">Date</span><span class="sxs-lookup"><span data-stu-id="4c387-112">Date</span></span>|<span data-ttu-id="4c387-113">Часть date метка времени.</span><span class="sxs-lookup"><span data-stu-id="4c387-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="4c387-114">time</span><span class="sxs-lookup"><span data-stu-id="4c387-114">time</span></span>|<span data-ttu-id="4c387-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4c387-115">TimeOfDay</span></span>|<span data-ttu-id="4c387-116">Часть времени метка времени.</span><span class="sxs-lookup"><span data-stu-id="4c387-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="4c387-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="4c387-117">timeZone</span></span>|<span data-ttu-id="4c387-118">Строка</span><span class="sxs-lookup"><span data-stu-id="4c387-118">String</span></span>|<span data-ttu-id="4c387-119">Часовой пояс часть метки времени — это один из 24 продольными областей в мире.</span><span class="sxs-lookup"><span data-stu-id="4c387-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
