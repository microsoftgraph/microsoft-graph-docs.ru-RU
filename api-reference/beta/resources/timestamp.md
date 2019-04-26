---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
ms.openlocfilehash: 5f96ad5c557bda93ef74787d9d909fce112cfb15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341955"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="dadc1-103">Тип ресурса timeStamp</span><span class="sxs-lookup"><span data-stu-id="dadc1-103">timeStamp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dadc1-104">Сведения о дате и времени для определенного момента времени.</span><span class="sxs-lookup"><span data-stu-id="dadc1-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dadc1-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dadc1-105">JSON representation</span></span>

<span data-ttu-id="dadc1-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="dadc1-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="dadc1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dadc1-107">Properties</span></span>
| <span data-ttu-id="dadc1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dadc1-108">Property</span></span>     | <span data-ttu-id="dadc1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dadc1-109">Type</span></span>   |<span data-ttu-id="dadc1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dadc1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dadc1-111">date</span><span class="sxs-lookup"><span data-stu-id="dadc1-111">date</span></span>|<span data-ttu-id="dadc1-112">Date</span><span class="sxs-lookup"><span data-stu-id="dadc1-112">Date</span></span>|<span data-ttu-id="dadc1-113">Часть даты метки времени.</span><span class="sxs-lookup"><span data-stu-id="dadc1-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="dadc1-114">time</span><span class="sxs-lookup"><span data-stu-id="dadc1-114">time</span></span>|<span data-ttu-id="dadc1-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="dadc1-115">TimeOfDay</span></span>|<span data-ttu-id="dadc1-116">Часть времени метки времени.</span><span class="sxs-lookup"><span data-stu-id="dadc1-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="dadc1-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="dadc1-117">timeZone</span></span>|<span data-ttu-id="dadc1-118">String</span><span class="sxs-lookup"><span data-stu-id="dadc1-118">String</span></span>|<span data-ttu-id="dadc1-119">Часть временной метки, представляющая часовой пояс (одна из 24 лонгитудинал областей мира).</span><span class="sxs-lookup"><span data-stu-id="dadc1-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
