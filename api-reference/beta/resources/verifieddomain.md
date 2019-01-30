---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
ms.openlocfilehash: c13c3b3da39b762c26d637deaddafbee5da40160
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641325"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="e8552-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="e8552-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8552-p102">Задает домен клиента. Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="e8552-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="e8552-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8552-107">Properties</span></span>
| <span data-ttu-id="e8552-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8552-108">Property</span></span>     | <span data-ttu-id="e8552-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e8552-109">Type</span></span>   |<span data-ttu-id="e8552-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e8552-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8552-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="e8552-111">capabilities</span></span>|<span data-ttu-id="e8552-112">String</span><span class="sxs-lookup"><span data-stu-id="e8552-112">String</span></span>|<span data-ttu-id="e8552-113">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="e8552-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="e8552-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="e8552-114">isDefault</span></span>|<span data-ttu-id="e8552-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8552-115">Boolean</span></span>|                <span data-ttu-id="e8552-116">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="e8552-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="e8552-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="e8552-117">isInitial</span></span>|<span data-ttu-id="e8552-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8552-118">Boolean</span></span>|<span data-ttu-id="e8552-119">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="e8552-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="e8552-120">name</span><span class="sxs-lookup"><span data-stu-id="e8552-120">name</span></span>|<span data-ttu-id="e8552-121">String</span><span class="sxs-lookup"><span data-stu-id="e8552-121">String</span></span>|<span data-ttu-id="e8552-122">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="e8552-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="e8552-123">type</span><span class="sxs-lookup"><span data-stu-id="e8552-123">type</span></span>|<span data-ttu-id="e8552-124">String</span><span class="sxs-lookup"><span data-stu-id="e8552-124">String</span></span>|<span data-ttu-id="e8552-125">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="e8552-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8552-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8552-126">JSON representation</span></span>

<span data-ttu-id="e8552-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8552-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/verifieddomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
