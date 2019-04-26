---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемый формат — Windows, а часовой пояс IP Numbers Authority (IANA) (также известный как часовой пояс Олсона).
localization_priority: Normal
ms.openlocfilehash: ecc13a614aacbe66e3e477bc87f874c215d10574
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341831"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="d0378-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="d0378-104">timeZoneInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0378-105">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="d0378-105">Represents a time zone.</span></span> <span data-ttu-id="d0378-106">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="d0378-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="d0378-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0378-107">Properties</span></span>
| <span data-ttu-id="d0378-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0378-108">Property</span></span>     | <span data-ttu-id="d0378-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0378-109">Type</span></span>   |<span data-ttu-id="d0378-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0378-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0378-111">alias</span><span class="sxs-lookup"><span data-stu-id="d0378-111">alias</span></span>|<span data-ttu-id="d0378-112">string</span><span class="sxs-lookup"><span data-stu-id="d0378-112">string</span></span>|<span data-ttu-id="d0378-113">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="d0378-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="d0378-114">displayName</span><span class="sxs-lookup"><span data-stu-id="d0378-114">displayName</span></span>|<span data-ttu-id="d0378-115">string</span><span class="sxs-lookup"><span data-stu-id="d0378-115">string</span></span>|<span data-ttu-id="d0378-116">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="d0378-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0378-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0378-117">JSON representation</span></span>

<span data-ttu-id="d0378-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0378-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
