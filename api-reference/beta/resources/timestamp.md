---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: JeremyKelley
ms.openlocfilehash: 295c4c8b4cee6ba476b5bae57ebd71de8d107c1c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075422"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="adfbf-103">Тип ресурса timeStamp</span><span class="sxs-lookup"><span data-stu-id="adfbf-103">timeStamp resource type</span></span>

<span data-ttu-id="adfbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adfbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adfbf-105">Сведения о дате и времени для определенного момента времени.</span><span class="sxs-lookup"><span data-stu-id="adfbf-105">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adfbf-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adfbf-106">JSON representation</span></span>

<span data-ttu-id="adfbf-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="adfbf-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="adfbf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="adfbf-108">Properties</span></span>
| <span data-ttu-id="adfbf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="adfbf-109">Property</span></span>     | <span data-ttu-id="adfbf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="adfbf-110">Type</span></span>   |<span data-ttu-id="adfbf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="adfbf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adfbf-112">date</span><span class="sxs-lookup"><span data-stu-id="adfbf-112">date</span></span>|<span data-ttu-id="adfbf-113">Date</span><span class="sxs-lookup"><span data-stu-id="adfbf-113">Date</span></span>|<span data-ttu-id="adfbf-114">Часть даты метки времени.</span><span class="sxs-lookup"><span data-stu-id="adfbf-114">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="adfbf-115">time</span><span class="sxs-lookup"><span data-stu-id="adfbf-115">time</span></span>|<span data-ttu-id="adfbf-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="adfbf-116">TimeOfDay</span></span>|<span data-ttu-id="adfbf-117">Часть времени метки времени.</span><span class="sxs-lookup"><span data-stu-id="adfbf-117">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="adfbf-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="adfbf-118">timeZone</span></span>|<span data-ttu-id="adfbf-119">String</span><span class="sxs-lookup"><span data-stu-id="adfbf-119">String</span></span>|<span data-ttu-id="adfbf-120">Часть временной метки, представляющая часовой пояс (одна из 24 лонгитудинал областей мира).</span><span class="sxs-lookup"><span data-stu-id="adfbf-120">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

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


