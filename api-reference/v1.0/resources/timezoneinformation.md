---
title: Тип ресурса timeZoneInformation
description: 'Представляет часовой пояс. Поддерживаемый формат : Windows и часовой пояс IANA (также известный как часовой пояс Олсон)'
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 146ea2e965368a7b025a83038e7377e6379bf4a2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136635"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="8cebd-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="8cebd-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="8cebd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cebd-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="8cebd-106">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="8cebd-106">Represents a time zone.</span></span> <span data-ttu-id="8cebd-107">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="8cebd-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="8cebd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cebd-108">Properties</span></span>
| <span data-ttu-id="8cebd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cebd-109">Property</span></span>     | <span data-ttu-id="8cebd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8cebd-110">Type</span></span>   |<span data-ttu-id="8cebd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8cebd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cebd-112">alias</span><span class="sxs-lookup"><span data-stu-id="8cebd-112">alias</span></span>|<span data-ttu-id="8cebd-113">string</span><span class="sxs-lookup"><span data-stu-id="8cebd-113">string</span></span>|<span data-ttu-id="8cebd-114">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="8cebd-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="8cebd-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8cebd-115">displayName</span></span>|<span data-ttu-id="8cebd-116">string</span><span class="sxs-lookup"><span data-stu-id="8cebd-116">string</span></span>|<span data-ttu-id="8cebd-117">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="8cebd-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cebd-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cebd-118">JSON representation</span></span>

<span data-ttu-id="8cebd-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cebd-119">Here is a JSON representation of the resource.</span></span>

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

