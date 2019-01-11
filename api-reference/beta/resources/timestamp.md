---
title: Тип ресурса метки времени
description: Дата и время сведения о времени.
localization_priority: Normal
ms.openlocfilehash: b3e6e7384c9efdcb0e606f91d7357272f27ceaa1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830228"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="80800-103">Тип ресурса метки времени</span><span class="sxs-lookup"><span data-stu-id="80800-103">timeStamp resource type</span></span>

> <span data-ttu-id="80800-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="80800-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80800-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80800-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80800-106">Дата и время сведения о времени.</span><span class="sxs-lookup"><span data-stu-id="80800-106">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80800-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80800-107">JSON representation</span></span>

<span data-ttu-id="80800-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="80800-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="80800-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="80800-109">Properties</span></span>
| <span data-ttu-id="80800-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="80800-110">Property</span></span>     | <span data-ttu-id="80800-111">Тип</span><span class="sxs-lookup"><span data-stu-id="80800-111">Type</span></span>   |<span data-ttu-id="80800-112">Описание</span><span class="sxs-lookup"><span data-stu-id="80800-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80800-113">date</span><span class="sxs-lookup"><span data-stu-id="80800-113">date</span></span>|<span data-ttu-id="80800-114">Date</span><span class="sxs-lookup"><span data-stu-id="80800-114">Date</span></span>|<span data-ttu-id="80800-115">Часть date метка времени.</span><span class="sxs-lookup"><span data-stu-id="80800-115">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="80800-116">time</span><span class="sxs-lookup"><span data-stu-id="80800-116">time</span></span>|<span data-ttu-id="80800-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="80800-117">TimeOfDay</span></span>|<span data-ttu-id="80800-118">Часть времени метка времени.</span><span class="sxs-lookup"><span data-stu-id="80800-118">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="80800-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="80800-119">timeZone</span></span>|<span data-ttu-id="80800-120">Строка</span><span class="sxs-lookup"><span data-stu-id="80800-120">String</span></span>|<span data-ttu-id="80800-121">Часовой пояс часть метки времени — это один из 24 продольными областей в мире.</span><span class="sxs-lookup"><span data-stu-id="80800-121">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
