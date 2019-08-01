---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемый формат — Windows, а часовой пояс IP Numbers Authority (IANA) (также известный как часовой пояс Олсона).
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9a1efdb217b6f4970cf0925aa69ebb50f451e938
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033553"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="79613-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="79613-104">timeZoneInformation resource type</span></span>


<span data-ttu-id="79613-105">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="79613-105">Represents a time zone.</span></span> <span data-ttu-id="79613-106">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="79613-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="79613-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="79613-107">Properties</span></span>
| <span data-ttu-id="79613-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="79613-108">Property</span></span>     | <span data-ttu-id="79613-109">Тип</span><span class="sxs-lookup"><span data-stu-id="79613-109">Type</span></span>   |<span data-ttu-id="79613-110">Описание</span><span class="sxs-lookup"><span data-stu-id="79613-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79613-111">alias</span><span class="sxs-lookup"><span data-stu-id="79613-111">alias</span></span>|<span data-ttu-id="79613-112">string</span><span class="sxs-lookup"><span data-stu-id="79613-112">string</span></span>|<span data-ttu-id="79613-113">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="79613-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="79613-114">displayName</span><span class="sxs-lookup"><span data-stu-id="79613-114">displayName</span></span>|<span data-ttu-id="79613-115">string</span><span class="sxs-lookup"><span data-stu-id="79613-115">string</span></span>|<span data-ttu-id="79613-116">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="79613-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79613-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79613-117">JSON representation</span></span>

<span data-ttu-id="79613-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79613-118">Here is a JSON representation of the resource.</span></span>

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
