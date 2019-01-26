---
title: Тип ресурса sharingDetail
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 380db80f120b29a0d1dca1a4b052679e483bc6f7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571039"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="44e8c-103">Тип ресурса sharingDetail</span><span class="sxs-lookup"><span data-stu-id="44e8c-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44e8c-104">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="44e8c-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="44e8c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44e8c-105">JSON representation</span></span>
<span data-ttu-id="44e8c-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="44e8c-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="44e8c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="44e8c-107">Properties</span></span>

| <span data-ttu-id="44e8c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="44e8c-108">Property</span></span>              | <span data-ttu-id="44e8c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="44e8c-109">Type</span></span>          | <span data-ttu-id="44e8c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="44e8c-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="44e8c-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="44e8c-111">sharedDateTime</span></span>        | <span data-ttu-id="44e8c-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44e8c-112">DateTimeOffset</span></span>| <span data-ttu-id="44e8c-113">Дата и время последнего общий файл.</span><span class="sxs-lookup"><span data-stu-id="44e8c-113">The date and time the file was last shared.</span></span> <span data-ttu-id="44e8c-114">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="44e8c-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="44e8c-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="44e8c-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="44e8c-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44e8c-116">Read-only.</span></span>  |
| <span data-ttu-id="44e8c-117">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="44e8c-117">sharingSubject</span></span>        | <span data-ttu-id="44e8c-118">Строка</span><span class="sxs-lookup"><span data-stu-id="44e8c-118">String</span></span>          | <span data-ttu-id="44e8c-119">Тема, с которым предоставлен общий доступ в документе.</span><span class="sxs-lookup"><span data-stu-id="44e8c-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="44e8c-120">sharingType</span><span class="sxs-lookup"><span data-stu-id="44e8c-120">sharingType</span></span>             | <span data-ttu-id="44e8c-121">Строка</span><span class="sxs-lookup"><span data-stu-id="44e8c-121">String</span></span>        | <span data-ttu-id="44e8c-122">Определяет способ документ предоставлен общий доступ, может быть «Ссылка», «Вложения», «Группа», «Сайт».</span><span class="sxs-lookup"><span data-stu-id="44e8c-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="44e8c-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="44e8c-123">sharedBy</span></span>                | [<span data-ttu-id="44e8c-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="44e8c-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="44e8c-125">Пользователь, общих документов.</span><span class="sxs-lookup"><span data-stu-id="44e8c-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="44e8c-126">sharingReference</span><span class="sxs-lookup"><span data-stu-id="44e8c-126">sharingReference</span></span>        | [<span data-ttu-id="44e8c-127">resourceReference</span><span class="sxs-lookup"><span data-stu-id="44e8c-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-sharingdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
