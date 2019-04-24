---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b5cfe363922fe466eef7a7333ce81249311b4063
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506869"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="81167-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="81167-105">educationTerm resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81167-106">Срок.</span><span class="sxs-lookup"><span data-stu-id="81167-106">A term.</span></span> <span data-ttu-id="81167-107">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="81167-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="81167-108">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="81167-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="81167-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="81167-109">Properties</span></span>
| <span data-ttu-id="81167-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="81167-110">Property</span></span>     | <span data-ttu-id="81167-111">Тип</span><span class="sxs-lookup"><span data-stu-id="81167-111">Type</span></span>   |<span data-ttu-id="81167-112">Описание</span><span class="sxs-lookup"><span data-stu-id="81167-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81167-113">displayName</span><span class="sxs-lookup"><span data-stu-id="81167-113">displayName</span></span>| <span data-ttu-id="81167-114">String</span><span class="sxs-lookup"><span data-stu-id="81167-114">String</span></span>| <span data-ttu-id="81167-115">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="81167-115">Display name of the term.</span></span>| 
|<span data-ttu-id="81167-116">externalId</span><span class="sxs-lookup"><span data-stu-id="81167-116">externalId</span></span>|<span data-ttu-id="81167-117">String</span><span class="sxs-lookup"><span data-stu-id="81167-117">String</span></span>| <span data-ttu-id="81167-118">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="81167-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="81167-119">startDate</span><span class="sxs-lookup"><span data-stu-id="81167-119">startDate</span></span>|<span data-ttu-id="81167-120">Дата</span><span class="sxs-lookup"><span data-stu-id="81167-120">Date</span></span>|<span data-ttu-id="81167-121">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="81167-121">Start of the term.</span></span>|
|<span data-ttu-id="81167-122">endDate</span><span class="sxs-lookup"><span data-stu-id="81167-122">endDate</span></span>|<span data-ttu-id="81167-123">Date</span><span class="sxs-lookup"><span data-stu-id="81167-123">Date</span></span>|<span data-ttu-id="81167-124">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="81167-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81167-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81167-125">JSON representation</span></span>

<span data-ttu-id="81167-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81167-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationterm.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
