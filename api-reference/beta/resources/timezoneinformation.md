---
title: Тип ресурса timeZoneInformation
description: 'Представляет часовой пояс. Поддерживаемый формат: Windows и часовой пояс IANA (также известный как часовой пояс Олсон)'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 65b46cc10f7054695772f4af6b329359aab5fe85
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130222"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="e0f21-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="e0f21-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="e0f21-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0f21-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0f21-106">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="e0f21-106">Represents a time zone.</span></span> <span data-ttu-id="e0f21-107">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="e0f21-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="e0f21-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0f21-108">Properties</span></span>
| <span data-ttu-id="e0f21-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0f21-109">Property</span></span>     | <span data-ttu-id="e0f21-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e0f21-110">Type</span></span>   |<span data-ttu-id="e0f21-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0f21-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0f21-112">alias</span><span class="sxs-lookup"><span data-stu-id="e0f21-112">alias</span></span>|<span data-ttu-id="e0f21-113">string</span><span class="sxs-lookup"><span data-stu-id="e0f21-113">string</span></span>|<span data-ttu-id="e0f21-114">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e0f21-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="e0f21-115">displayName</span><span class="sxs-lookup"><span data-stu-id="e0f21-115">displayName</span></span>|<span data-ttu-id="e0f21-116">string</span><span class="sxs-lookup"><span data-stu-id="e0f21-116">string</span></span>|<span data-ttu-id="e0f21-117">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e0f21-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0f21-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e0f21-118">JSON representation</span></span>

<span data-ttu-id="e0f21-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0f21-119">Here is a JSON representation of the resource.</span></span>

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


