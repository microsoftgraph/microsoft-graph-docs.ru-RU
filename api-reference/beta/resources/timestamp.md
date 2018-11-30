---
title: Тип ресурса метки времени
description: Дата и время сведения о времени.
ms.openlocfilehash: 24326f0c104dd4ee2be80016ce798cc843288975
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078349"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="81ef7-103">Тип ресурса метки времени</span><span class="sxs-lookup"><span data-stu-id="81ef7-103">timeStamp resource type</span></span>

> <span data-ttu-id="81ef7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81ef7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81ef7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81ef7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81ef7-106">Дата и время сведения о времени.</span><span class="sxs-lookup"><span data-stu-id="81ef7-106">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81ef7-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81ef7-107">JSON representation</span></span>

<span data-ttu-id="81ef7-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="81ef7-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="81ef7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="81ef7-109">Properties</span></span>
| <span data-ttu-id="81ef7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="81ef7-110">Property</span></span>     | <span data-ttu-id="81ef7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="81ef7-111">Type</span></span>   |<span data-ttu-id="81ef7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="81ef7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81ef7-113">date</span><span class="sxs-lookup"><span data-stu-id="81ef7-113">date</span></span>|<span data-ttu-id="81ef7-114">Date</span><span class="sxs-lookup"><span data-stu-id="81ef7-114">Date</span></span>|<span data-ttu-id="81ef7-115">Часть date метка времени.</span><span class="sxs-lookup"><span data-stu-id="81ef7-115">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="81ef7-116">time</span><span class="sxs-lookup"><span data-stu-id="81ef7-116">time</span></span>|<span data-ttu-id="81ef7-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="81ef7-117">TimeOfDay</span></span>|<span data-ttu-id="81ef7-118">Часть времени метка времени.</span><span class="sxs-lookup"><span data-stu-id="81ef7-118">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="81ef7-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="81ef7-119">timeZone</span></span>|<span data-ttu-id="81ef7-120">String</span><span class="sxs-lookup"><span data-stu-id="81ef7-120">String</span></span>|<span data-ttu-id="81ef7-121">Часовой пояс часть метки времени — это один из 24 продольными областей в мире.</span><span class="sxs-lookup"><span data-stu-id="81ef7-121">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->