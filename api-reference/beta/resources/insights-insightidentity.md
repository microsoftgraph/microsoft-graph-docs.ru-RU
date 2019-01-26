---
title: insightIdentity
description: Сложный тип, содержащий свойства общих элементов.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 47283a82260d4f03a271a16660d58aca60da94e1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577230"
---
# <a name="insightidentity"></a><span data-ttu-id="c5fc0-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="c5fc0-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5fc0-104">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="c5fc0-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="c5fc0-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5fc0-105">JSON representation</span></span>
<span data-ttu-id="c5fc0-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c5fc0-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="c5fc0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5fc0-107">Properties</span></span>

| <span data-ttu-id="c5fc0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5fc0-108">Property</span></span>              | <span data-ttu-id="c5fc0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c5fc0-109">Type</span></span>          | <span data-ttu-id="c5fc0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5fc0-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="c5fc0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c5fc0-111">displayName</span></span>       | <span data-ttu-id="c5fc0-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c5fc0-112">String</span></span>          | <span data-ttu-id="c5fc0-113">Отображаемое имя пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="c5fc0-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="c5fc0-114">id</span><span class="sxs-lookup"><span data-stu-id="c5fc0-114">id</span></span>              | <span data-ttu-id="c5fc0-115">Строка</span><span class="sxs-lookup"><span data-stu-id="c5fc0-115">String</span></span>        | <span data-ttu-id="c5fc0-116">Идентификатор пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="c5fc0-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="c5fc0-117">address</span><span class="sxs-lookup"><span data-stu-id="c5fc0-117">address</span></span>             | <span data-ttu-id="c5fc0-118">String</span><span class="sxs-lookup"><span data-stu-id="c5fc0-118">String</span></span>      | <span data-ttu-id="c5fc0-119">Адрес электронной почты пользователя, который общих элемента.</span><span class="sxs-lookup"><span data-stu-id="c5fc0-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
