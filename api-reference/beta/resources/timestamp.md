---
title: Тип ресурса timeStamp
description: Сведения о дате и времени для определенного момента времени.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 72da26fa1e6dd428f53f2cb219a681a32a8ba42b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519696"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="d9249-103">Тип ресурса timeStamp</span><span class="sxs-lookup"><span data-stu-id="d9249-103">timeStamp resource type</span></span>

<span data-ttu-id="d9249-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9249-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9249-105">Сведения о дате и времени для определенного момента времени.</span><span class="sxs-lookup"><span data-stu-id="d9249-105">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9249-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9249-106">JSON representation</span></span>

<span data-ttu-id="d9249-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d9249-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d9249-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9249-108">Properties</span></span>
| <span data-ttu-id="d9249-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9249-109">Property</span></span>     | <span data-ttu-id="d9249-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d9249-110">Type</span></span>   |<span data-ttu-id="d9249-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9249-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9249-112">date</span><span class="sxs-lookup"><span data-stu-id="d9249-112">date</span></span>|<span data-ttu-id="d9249-113">Date</span><span class="sxs-lookup"><span data-stu-id="d9249-113">Date</span></span>|<span data-ttu-id="d9249-114">Часть даты метки времени.</span><span class="sxs-lookup"><span data-stu-id="d9249-114">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="d9249-115">time</span><span class="sxs-lookup"><span data-stu-id="d9249-115">time</span></span>|<span data-ttu-id="d9249-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d9249-116">TimeOfDay</span></span>|<span data-ttu-id="d9249-117">Часть времени метки времени.</span><span class="sxs-lookup"><span data-stu-id="d9249-117">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="d9249-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="d9249-118">timeZone</span></span>|<span data-ttu-id="d9249-119">String</span><span class="sxs-lookup"><span data-stu-id="d9249-119">String</span></span>|<span data-ttu-id="d9249-120">Часть временной метки, представляющая часовой пояс (одна из 24 лонгитудинал областей мира).</span><span class="sxs-lookup"><span data-stu-id="d9249-120">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

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
