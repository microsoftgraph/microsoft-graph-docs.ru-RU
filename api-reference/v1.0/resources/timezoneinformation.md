---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемые формата является Windows и Internet Assigned Numbers Authority (IANA) часовой пояс (также известной как Олсон часовой пояс)
localization_priority: Normal
ms.openlocfilehash: ced18a28a5c086416fa7247e1531d772fd63b977
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830200"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="a918a-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="a918a-104">timeZoneInformation resource type</span></span>


<span data-ttu-id="a918a-105">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="a918a-105">Represents a time zone.</span></span> <span data-ttu-id="a918a-106">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="a918a-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="a918a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a918a-107">Properties</span></span>
| <span data-ttu-id="a918a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a918a-108">Property</span></span>     | <span data-ttu-id="a918a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a918a-109">Type</span></span>   |<span data-ttu-id="a918a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a918a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a918a-111">alias</span><span class="sxs-lookup"><span data-stu-id="a918a-111">alias</span></span>|<span data-ttu-id="a918a-112">string</span><span class="sxs-lookup"><span data-stu-id="a918a-112">string</span></span>|<span data-ttu-id="a918a-113">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a918a-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="a918a-114">displayName</span><span class="sxs-lookup"><span data-stu-id="a918a-114">displayName</span></span>|<span data-ttu-id="a918a-115">строка</span><span class="sxs-lookup"><span data-stu-id="a918a-115">string</span></span>|<span data-ttu-id="a918a-116">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="a918a-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a918a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a918a-117">JSON representation</span></span>

<span data-ttu-id="a918a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a918a-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
