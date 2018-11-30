---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемые формата является Windows и Internet Assigned Numbers Authority (IANA) часовой пояс (также известной как Олсон часовой пояс)
ms.openlocfilehash: 5508f20812b8327a068364df7eb33c5072c3512e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078339"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="acbcc-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="acbcc-104">timeZoneInformation resource type</span></span>

> <span data-ttu-id="acbcc-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="acbcc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acbcc-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acbcc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="acbcc-107">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="acbcc-107">Represents a time zone.</span></span> <span data-ttu-id="acbcc-108">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="acbcc-108">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="acbcc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="acbcc-109">Properties</span></span>
| <span data-ttu-id="acbcc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="acbcc-110">Property</span></span>     | <span data-ttu-id="acbcc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="acbcc-111">Type</span></span>   |<span data-ttu-id="acbcc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="acbcc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acbcc-113">alias</span><span class="sxs-lookup"><span data-stu-id="acbcc-113">alias</span></span>|<span data-ttu-id="acbcc-114">string</span><span class="sxs-lookup"><span data-stu-id="acbcc-114">string</span></span>|<span data-ttu-id="acbcc-115">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="acbcc-115">An identifier for the time zone.</span></span>|
|<span data-ttu-id="acbcc-116">displayName</span><span class="sxs-lookup"><span data-stu-id="acbcc-116">displayName</span></span>|<span data-ttu-id="acbcc-117">строка</span><span class="sxs-lookup"><span data-stu-id="acbcc-117">string</span></span>|<span data-ttu-id="acbcc-118">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="acbcc-118">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="acbcc-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="acbcc-119">JSON representation</span></span>

<span data-ttu-id="acbcc-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acbcc-120">Here is a JSON representation of the resource.</span></span>

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