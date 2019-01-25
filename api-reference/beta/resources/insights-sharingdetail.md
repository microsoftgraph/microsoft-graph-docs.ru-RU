---
title: Тип ресурса sharingDetail
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 3fff669b2b337e9566cd41a7cd5eb5ab73a84944
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512271"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="5e8cb-103">Тип ресурса sharingDetail</span><span class="sxs-lookup"><span data-stu-id="5e8cb-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e8cb-104">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="5e8cb-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="5e8cb-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e8cb-105">JSON representation</span></span>
<span data-ttu-id="5e8cb-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="5e8cb-106">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="5e8cb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e8cb-107">Properties</span></span>

| <span data-ttu-id="5e8cb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e8cb-108">Property</span></span>              | <span data-ttu-id="5e8cb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5e8cb-109">Type</span></span>          | <span data-ttu-id="5e8cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e8cb-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="5e8cb-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e8cb-111">sharedDateTime</span></span>        | <span data-ttu-id="5e8cb-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e8cb-112">DateTimeOffset</span></span>| <span data-ttu-id="5e8cb-113">Дата и время последнего общий файл.</span><span class="sxs-lookup"><span data-stu-id="5e8cb-113">The date and time the file was last shared.</span></span> <span data-ttu-id="5e8cb-114">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5e8cb-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e8cb-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5e8cb-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="5e8cb-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e8cb-116">Read-only.</span></span>  |
| <span data-ttu-id="5e8cb-117">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="5e8cb-117">sharingSubject</span></span>        | <span data-ttu-id="5e8cb-118">String</span><span class="sxs-lookup"><span data-stu-id="5e8cb-118">String</span></span>          | <span data-ttu-id="5e8cb-119">Тема, с которым предоставлен общий доступ в документе.</span><span class="sxs-lookup"><span data-stu-id="5e8cb-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="5e8cb-120">SharingType</span><span class="sxs-lookup"><span data-stu-id="5e8cb-120">sharingType</span></span>             | <span data-ttu-id="5e8cb-121">String</span><span class="sxs-lookup"><span data-stu-id="5e8cb-121">String</span></span>        | <span data-ttu-id="5e8cb-122">Определяет способ документ предоставлен общий доступ, может быть «Ссылка», «Вложения», «Группа», «Сайт».</span><span class="sxs-lookup"><span data-stu-id="5e8cb-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="5e8cb-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="5e8cb-123">sharedBy</span></span>                | [<span data-ttu-id="5e8cb-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="5e8cb-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="5e8cb-125">Пользователь, общих документов.</span><span class="sxs-lookup"><span data-stu-id="5e8cb-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="5e8cb-126">sharingReference</span><span class="sxs-lookup"><span data-stu-id="5e8cb-126">sharingReference</span></span>        | [<span data-ttu-id="5e8cb-127">resourceReference</span><span class="sxs-lookup"><span data-stu-id="5e8cb-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-sharingdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
