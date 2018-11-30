---
title: Тип ресурса метки времени
description: Дата и время сведения о времени.
ms.openlocfilehash: 4f392e880bb165841fd8a9a31b6ed00bf2ba36fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025132"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="6d802-103">Тип ресурса метки времени</span><span class="sxs-lookup"><span data-stu-id="6d802-103">timeStamp resource type</span></span>

<span data-ttu-id="6d802-104">Дата и время сведения о времени.</span><span class="sxs-lookup"><span data-stu-id="6d802-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d802-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d802-105">JSON representation</span></span>

<span data-ttu-id="6d802-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6d802-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6d802-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d802-107">Properties</span></span>
| <span data-ttu-id="6d802-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d802-108">Property</span></span>       | <span data-ttu-id="6d802-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6d802-109">Type</span></span>    |<span data-ttu-id="6d802-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6d802-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d802-111">date</span><span class="sxs-lookup"><span data-stu-id="6d802-111">date</span></span>|<span data-ttu-id="6d802-112">Date</span><span class="sxs-lookup"><span data-stu-id="6d802-112">Date</span></span>|<span data-ttu-id="6d802-113">Часть date метка времени.</span><span class="sxs-lookup"><span data-stu-id="6d802-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="6d802-114">time</span><span class="sxs-lookup"><span data-stu-id="6d802-114">time</span></span>|<span data-ttu-id="6d802-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6d802-115">TimeOfDay</span></span>|<span data-ttu-id="6d802-116">Часть времени метка времени.</span><span class="sxs-lookup"><span data-stu-id="6d802-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="6d802-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="6d802-117">timeZone</span></span>|<span data-ttu-id="6d802-118">String</span><span class="sxs-lookup"><span data-stu-id="6d802-118">String</span></span>|<span data-ttu-id="6d802-119">Часовой пояс часть метки времени — это один из 24 продольными областей в мире.</span><span class="sxs-lookup"><span data-stu-id="6d802-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->