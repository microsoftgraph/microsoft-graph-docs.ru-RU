---
title: Тип ресурса Шарингдетаил
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c62fc11c668a5175e0dafa9bdf4c937fecbef798
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005718"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="ceb7f-103">Тип ресурса Шарингдетаил</span><span class="sxs-lookup"><span data-stu-id="ceb7f-103">sharingDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceb7f-104">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="ceb7f-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="ceb7f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ceb7f-105">JSON representation</span></span>
<span data-ttu-id="ceb7f-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ceb7f-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="ceb7f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ceb7f-107">Properties</span></span>

| <span data-ttu-id="ceb7f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ceb7f-108">Property</span></span>              | <span data-ttu-id="ceb7f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ceb7f-109">Type</span></span>          | <span data-ttu-id="ceb7f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ceb7f-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="ceb7f-111">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="ceb7f-111">sharedDateTime</span></span>        | <span data-ttu-id="ceb7f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceb7f-112">DateTimeOffset</span></span>| <span data-ttu-id="ceb7f-113">Дата и время последнего предоставления общего доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="ceb7f-113">The date and time the file was last shared.</span></span> <span data-ttu-id="ceb7f-114">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ceb7f-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ceb7f-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ceb7f-115">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="ceb7f-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ceb7f-116">Read-only.</span></span>  |
| <span data-ttu-id="ceb7f-117">Шарингсубжект</span><span class="sxs-lookup"><span data-stu-id="ceb7f-117">sharingSubject</span></span>        | <span data-ttu-id="ceb7f-118">String</span><span class="sxs-lookup"><span data-stu-id="ceb7f-118">String</span></span>          | <span data-ttu-id="ceb7f-119">Тема, к которой был предоставлен общий доступ к документу.</span><span class="sxs-lookup"><span data-stu-id="ceb7f-119">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="ceb7f-120">Шарингтипе</span><span class="sxs-lookup"><span data-stu-id="ceb7f-120">sharingType</span></span>             | <span data-ttu-id="ceb7f-121">String</span><span class="sxs-lookup"><span data-stu-id="ceb7f-121">String</span></span>        | <span data-ttu-id="ceb7f-122">Определяет способ предоставления общего доступа к документу, который может быть "ссылка", "вложение", "Группа", "сайт".</span><span class="sxs-lookup"><span data-stu-id="ceb7f-122">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="ceb7f-123">sharedBy</span><span class="sxs-lookup"><span data-stu-id="ceb7f-123">sharedBy</span></span>                | [<span data-ttu-id="ceb7f-124">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="ceb7f-124">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="ceb7f-125">Пользователь, имеющий общий доступ к документу.</span><span class="sxs-lookup"><span data-stu-id="ceb7f-125">The user who shared the document.</span></span>  |
| <span data-ttu-id="ceb7f-126">Шарингреференце</span><span class="sxs-lookup"><span data-stu-id="ceb7f-126">sharingReference</span></span>        | [<span data-ttu-id="ceb7f-127">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="ceb7f-127">resourceReference</span></span>](insights-resourcereference.md)      |  |
