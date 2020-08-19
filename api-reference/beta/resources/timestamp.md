---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: JeremyKelley
ms.openlocfilehash: 1037212f1adb0fb10326bbdf88416877e16a9fbe
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810995"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="c141e-103">Тип ресурса timeStamp</span><span class="sxs-lookup"><span data-stu-id="c141e-103">timeStamp resource type</span></span>

<span data-ttu-id="c141e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c141e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c141e-105">Сведения о дате и времени для определенного момента времени.</span><span class="sxs-lookup"><span data-stu-id="c141e-105">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c141e-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c141e-106">JSON representation</span></span>

<span data-ttu-id="c141e-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c141e-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="c141e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c141e-108">Properties</span></span>
| <span data-ttu-id="c141e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c141e-109">Property</span></span>     | <span data-ttu-id="c141e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c141e-110">Type</span></span>   |<span data-ttu-id="c141e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c141e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c141e-112">date</span><span class="sxs-lookup"><span data-stu-id="c141e-112">date</span></span>|<span data-ttu-id="c141e-113">Date</span><span class="sxs-lookup"><span data-stu-id="c141e-113">Date</span></span>|<span data-ttu-id="c141e-114">Часть даты метки времени.</span><span class="sxs-lookup"><span data-stu-id="c141e-114">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="c141e-115">time</span><span class="sxs-lookup"><span data-stu-id="c141e-115">time</span></span>|<span data-ttu-id="c141e-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c141e-116">TimeOfDay</span></span>|<span data-ttu-id="c141e-117">Часть времени метки времени.</span><span class="sxs-lookup"><span data-stu-id="c141e-117">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="c141e-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="c141e-118">timeZone</span></span>|<span data-ttu-id="c141e-119">String</span><span class="sxs-lookup"><span data-stu-id="c141e-119">String</span></span>|<span data-ttu-id="c141e-120">Часть временной метки, представляющая часовой пояс (одна из 24 лонгитудинал областей мира).</span><span class="sxs-lookup"><span data-stu-id="c141e-120">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

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
