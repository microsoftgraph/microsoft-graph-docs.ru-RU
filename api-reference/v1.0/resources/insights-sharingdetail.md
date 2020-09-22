---
title: Тип ресурса Шарингдетаил
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 0540ebae50cb766b25daaad6e80d8b3248e79e42
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054793"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="e0b4c-103">Тип ресурса Шарингдетаил</span><span class="sxs-lookup"><span data-stu-id="e0b4c-103">sharingDetail resource type</span></span>

<span data-ttu-id="e0b4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0b4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0b4c-105">Сложный тип, содержащий свойства элементов [шарединсигхт](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="e0b4c-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="e0b4c-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0b4c-106">JSON representation</span></span>
<span data-ttu-id="e0b4c-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0b4c-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="e0b4c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0b4c-108">Properties</span></span>

| <span data-ttu-id="e0b4c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0b4c-109">Property</span></span>              | <span data-ttu-id="e0b4c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e0b4c-110">Type</span></span>          | <span data-ttu-id="e0b4c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0b4c-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="e0b4c-112">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b4c-112">sharedDateTime</span></span>        | <span data-ttu-id="e0b4c-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0b4c-113">DateTimeOffset</span></span>| <span data-ttu-id="e0b4c-114">Дата и время последнего предоставления общего доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="e0b4c-114">The date and time the file was last shared.</span></span> <span data-ttu-id="e0b4c-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e0b4c-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0b4c-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e0b4c-116">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e0b4c-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0b4c-117">Read-only.</span></span>  |
| <span data-ttu-id="e0b4c-118">шарингсубжект</span><span class="sxs-lookup"><span data-stu-id="e0b4c-118">sharingSubject</span></span>        | <span data-ttu-id="e0b4c-119">String</span><span class="sxs-lookup"><span data-stu-id="e0b4c-119">String</span></span>          | <span data-ttu-id="e0b4c-120">Тема, к которой был предоставлен общий доступ к документу.</span><span class="sxs-lookup"><span data-stu-id="e0b4c-120">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="e0b4c-121">шарингтипе</span><span class="sxs-lookup"><span data-stu-id="e0b4c-121">sharingType</span></span>             | <span data-ttu-id="e0b4c-122">String</span><span class="sxs-lookup"><span data-stu-id="e0b4c-122">String</span></span>        | <span data-ttu-id="e0b4c-123">Определяет способ предоставления общего доступа к документу, который может быть "ссылка", "вложение", "Группа", "сайт".</span><span class="sxs-lookup"><span data-stu-id="e0b4c-123">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="e0b4c-124">sharedBy</span><span class="sxs-lookup"><span data-stu-id="e0b4c-124">sharedBy</span></span>                | [<span data-ttu-id="e0b4c-125">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="e0b4c-125">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="e0b4c-126">Пользователь, имеющий общий доступ к документу.</span><span class="sxs-lookup"><span data-stu-id="e0b4c-126">The user who shared the document.</span></span>  |
| <span data-ttu-id="e0b4c-127">шарингреференце</span><span class="sxs-lookup"><span data-stu-id="e0b4c-127">sharingReference</span></span>        | [<span data-ttu-id="e0b4c-128">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="e0b4c-128">resourceReference</span></span>](insights-resourcereference.md)      |  |

