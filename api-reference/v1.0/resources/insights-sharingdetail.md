---
title: Тип ресурса Шарингдетаил
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c441dcdc3b743e5bf55786ad1b43bfe2010b01b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531289"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="32737-103">Тип ресурса Шарингдетаил</span><span class="sxs-lookup"><span data-stu-id="32737-103">sharingDetail resource type</span></span>

<span data-ttu-id="32737-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32737-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32737-105">Сложный тип, содержащий свойства элементов [шарединсигхт](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="32737-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="32737-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32737-106">JSON representation</span></span>
<span data-ttu-id="32737-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="32737-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="32737-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="32737-108">Properties</span></span>

| <span data-ttu-id="32737-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="32737-109">Property</span></span>              | <span data-ttu-id="32737-110">Тип</span><span class="sxs-lookup"><span data-stu-id="32737-110">Type</span></span>          | <span data-ttu-id="32737-111">Описание</span><span class="sxs-lookup"><span data-stu-id="32737-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="32737-112">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="32737-112">sharedDateTime</span></span>        | <span data-ttu-id="32737-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32737-113">DateTimeOffset</span></span>| <span data-ttu-id="32737-114">Дата и время последнего предоставления общего доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="32737-114">The date and time the file was last shared.</span></span> <span data-ttu-id="32737-115">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="32737-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="32737-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="32737-116">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="32737-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32737-117">Read-only.</span></span>  |
| <span data-ttu-id="32737-118">шарингсубжект</span><span class="sxs-lookup"><span data-stu-id="32737-118">sharingSubject</span></span>        | <span data-ttu-id="32737-119">String</span><span class="sxs-lookup"><span data-stu-id="32737-119">String</span></span>          | <span data-ttu-id="32737-120">Тема, к которой был предоставлен общий доступ к документу.</span><span class="sxs-lookup"><span data-stu-id="32737-120">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="32737-121">шарингтипе</span><span class="sxs-lookup"><span data-stu-id="32737-121">sharingType</span></span>             | <span data-ttu-id="32737-122">String</span><span class="sxs-lookup"><span data-stu-id="32737-122">String</span></span>        | <span data-ttu-id="32737-123">Определяет способ предоставления общего доступа к документу, который может быть "ссылка", "вложение", "Группа", "сайт".</span><span class="sxs-lookup"><span data-stu-id="32737-123">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="32737-124">sharedBy</span><span class="sxs-lookup"><span data-stu-id="32737-124">sharedBy</span></span>                | [<span data-ttu-id="32737-125">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="32737-125">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="32737-126">Пользователь, имеющий общий доступ к документу.</span><span class="sxs-lookup"><span data-stu-id="32737-126">The user who shared the document.</span></span>  |
| <span data-ttu-id="32737-127">шарингреференце</span><span class="sxs-lookup"><span data-stu-id="32737-127">sharingReference</span></span>        | [<span data-ttu-id="32737-128">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="32737-128">resourceReference</span></span>](insights-resourcereference.md)      |  |
