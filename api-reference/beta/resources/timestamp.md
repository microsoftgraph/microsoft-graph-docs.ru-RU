---
title: Тип ресурса метки времени
description: Дата и время сведения о времени.
localization_priority: Normal
ms.openlocfilehash: 79faa8f74fbaf64eb6756183ecc309c6522873e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529364"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="8c26e-103">Тип ресурса метки времени</span><span class="sxs-lookup"><span data-stu-id="8c26e-103">timeStamp resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c26e-104">Дата и время сведения о времени.</span><span class="sxs-lookup"><span data-stu-id="8c26e-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c26e-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c26e-105">JSON representation</span></span>

<span data-ttu-id="8c26e-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8c26e-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8c26e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c26e-107">Properties</span></span>
| <span data-ttu-id="8c26e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c26e-108">Property</span></span>     | <span data-ttu-id="8c26e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8c26e-109">Type</span></span>   |<span data-ttu-id="8c26e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c26e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c26e-111">дата</span><span class="sxs-lookup"><span data-stu-id="8c26e-111">date</span></span>|<span data-ttu-id="8c26e-112">Date</span><span class="sxs-lookup"><span data-stu-id="8c26e-112">Date</span></span>|<span data-ttu-id="8c26e-113">Часть date метка времени.</span><span class="sxs-lookup"><span data-stu-id="8c26e-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="8c26e-114">time</span><span class="sxs-lookup"><span data-stu-id="8c26e-114">time</span></span>|<span data-ttu-id="8c26e-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8c26e-115">TimeOfDay</span></span>|<span data-ttu-id="8c26e-116">Часть времени метка времени.</span><span class="sxs-lookup"><span data-stu-id="8c26e-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="8c26e-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="8c26e-117">timeZone</span></span>|<span data-ttu-id="8c26e-118">String</span><span class="sxs-lookup"><span data-stu-id="8c26e-118">String</span></span>|<span data-ttu-id="8c26e-119">Часовой пояс часть метки времени — это один из 24 продольными областей в мире.</span><span class="sxs-lookup"><span data-stu-id="8c26e-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timestamp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
