---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемый формат — Windows, а часовой пояс IP Numbers Authority (IANA) (также известный как часовой пояс Олсона).
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 81f1eb3f8abbdcf95b94407019807d0d002dc286
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811828"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="02c91-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="02c91-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="02c91-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02c91-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="02c91-106">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="02c91-106">Represents a time zone.</span></span> <span data-ttu-id="02c91-107">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="02c91-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="02c91-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="02c91-108">Properties</span></span>
| <span data-ttu-id="02c91-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="02c91-109">Property</span></span>     | <span data-ttu-id="02c91-110">Тип</span><span class="sxs-lookup"><span data-stu-id="02c91-110">Type</span></span>   |<span data-ttu-id="02c91-111">Описание</span><span class="sxs-lookup"><span data-stu-id="02c91-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02c91-112">alias</span><span class="sxs-lookup"><span data-stu-id="02c91-112">alias</span></span>|<span data-ttu-id="02c91-113">string</span><span class="sxs-lookup"><span data-stu-id="02c91-113">string</span></span>|<span data-ttu-id="02c91-114">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="02c91-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="02c91-115">displayName</span><span class="sxs-lookup"><span data-stu-id="02c91-115">displayName</span></span>|<span data-ttu-id="02c91-116">string</span><span class="sxs-lookup"><span data-stu-id="02c91-116">string</span></span>|<span data-ttu-id="02c91-117">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="02c91-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02c91-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="02c91-118">JSON representation</span></span>

<span data-ttu-id="02c91-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02c91-119">Here is a JSON representation of the resource.</span></span>

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
