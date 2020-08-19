---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0629eaabd282f03184be28ade67c2d17d5598602
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808146"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="d3787-103">Тип ресурса timeStamp</span><span class="sxs-lookup"><span data-stu-id="d3787-103">timeStamp resource type</span></span>

<span data-ttu-id="d3787-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3787-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3787-105">Сведения о дате и времени для определенного момента времени.</span><span class="sxs-lookup"><span data-stu-id="d3787-105">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3787-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d3787-106">JSON representation</span></span>

<span data-ttu-id="d3787-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d3787-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d3787-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3787-108">Properties</span></span>
| <span data-ttu-id="d3787-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3787-109">Property</span></span>       | <span data-ttu-id="d3787-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d3787-110">Type</span></span>    |<span data-ttu-id="d3787-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d3787-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3787-112">date</span><span class="sxs-lookup"><span data-stu-id="d3787-112">date</span></span>|<span data-ttu-id="d3787-113">Date</span><span class="sxs-lookup"><span data-stu-id="d3787-113">Date</span></span>|<span data-ttu-id="d3787-114">Часть даты метки времени.</span><span class="sxs-lookup"><span data-stu-id="d3787-114">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="d3787-115">time</span><span class="sxs-lookup"><span data-stu-id="d3787-115">time</span></span>|<span data-ttu-id="d3787-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d3787-116">TimeOfDay</span></span>|<span data-ttu-id="d3787-117">Часть времени метки времени.</span><span class="sxs-lookup"><span data-stu-id="d3787-117">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="d3787-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="d3787-118">timeZone</span></span>|<span data-ttu-id="d3787-119">String</span><span class="sxs-lookup"><span data-stu-id="d3787-119">String</span></span>|<span data-ttu-id="d3787-120">Часть временной метки, представляющая часовой пояс (одна из 24 лонгитудинал областей мира).</span><span class="sxs-lookup"><span data-stu-id="d3787-120">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
