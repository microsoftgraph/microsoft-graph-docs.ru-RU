---
title: Тип ресурса timeZoneInformation
description: Представляет часовой пояс. Поддерживаемый формат — Windows, а часовой пояс IP Numbers Authority (IANA) (также известный как часовой пояс Олсона).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3deae74f1ffc991e6e9178a46575c21d69272d2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519682"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="82bec-104">Тип ресурса timeZoneInformation</span><span class="sxs-lookup"><span data-stu-id="82bec-104">timeZoneInformation resource type</span></span>

<span data-ttu-id="82bec-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82bec-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82bec-106">Представляет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="82bec-106">Represents a time zone.</span></span> <span data-ttu-id="82bec-107">Поддерживаются формат Windows и формат [часового пояса IANA](https://www.iana.org/time-zones), также известного как часовой пояс Олсона (после устранения известной проблемы).</span><span class="sxs-lookup"><span data-stu-id="82bec-107">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="82bec-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="82bec-108">Properties</span></span>
| <span data-ttu-id="82bec-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="82bec-109">Property</span></span>     | <span data-ttu-id="82bec-110">Тип</span><span class="sxs-lookup"><span data-stu-id="82bec-110">Type</span></span>   |<span data-ttu-id="82bec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="82bec-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82bec-112">alias</span><span class="sxs-lookup"><span data-stu-id="82bec-112">alias</span></span>|<span data-ttu-id="82bec-113">string</span><span class="sxs-lookup"><span data-stu-id="82bec-113">string</span></span>|<span data-ttu-id="82bec-114">Идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="82bec-114">An identifier for the time zone.</span></span>|
|<span data-ttu-id="82bec-115">displayName</span><span class="sxs-lookup"><span data-stu-id="82bec-115">displayName</span></span>|<span data-ttu-id="82bec-116">string</span><span class="sxs-lookup"><span data-stu-id="82bec-116">string</span></span>|<span data-ttu-id="82bec-117">Отображаемое имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="82bec-117">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82bec-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="82bec-118">JSON representation</span></span>

<span data-ttu-id="82bec-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82bec-119">Here is a JSON representation of the resource.</span></span>

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
