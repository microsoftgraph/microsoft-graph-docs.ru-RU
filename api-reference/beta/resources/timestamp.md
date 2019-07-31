---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: cda000674241ee57347d6809d04d7acd9d59ff0b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964289"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="7f4c4-103">Тип ресурса timeStamp</span><span class="sxs-lookup"><span data-stu-id="7f4c4-103">timeStamp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f4c4-104">Сведения о дате и времени для определенного момента времени.</span><span class="sxs-lookup"><span data-stu-id="7f4c4-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f4c4-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f4c4-105">JSON representation</span></span>

<span data-ttu-id="7f4c4-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="7f4c4-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="7f4c4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f4c4-107">Properties</span></span>
| <span data-ttu-id="7f4c4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f4c4-108">Property</span></span>     | <span data-ttu-id="7f4c4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7f4c4-109">Type</span></span>   |<span data-ttu-id="7f4c4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f4c4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f4c4-111">date</span><span class="sxs-lookup"><span data-stu-id="7f4c4-111">date</span></span>|<span data-ttu-id="7f4c4-112">Date</span><span class="sxs-lookup"><span data-stu-id="7f4c4-112">Date</span></span>|<span data-ttu-id="7f4c4-113">Часть даты метки времени.</span><span class="sxs-lookup"><span data-stu-id="7f4c4-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="7f4c4-114">time</span><span class="sxs-lookup"><span data-stu-id="7f4c4-114">time</span></span>|<span data-ttu-id="7f4c4-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7f4c4-115">TimeOfDay</span></span>|<span data-ttu-id="7f4c4-116">Часть времени метки времени.</span><span class="sxs-lookup"><span data-stu-id="7f4c4-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="7f4c4-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="7f4c4-117">timeZone</span></span>|<span data-ttu-id="7f4c4-118">String</span><span class="sxs-lookup"><span data-stu-id="7f4c4-118">String</span></span>|<span data-ttu-id="7f4c4-119">Часть временной метки, представляющая часовой пояс (одна из 24 лонгитудинал областей мира).</span><span class="sxs-lookup"><span data-stu-id="7f4c4-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

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
