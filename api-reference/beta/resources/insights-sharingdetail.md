---
title: Тип ресурса sharingDetail
description: 'Сложный тип, содержащий свойства общих элементов. '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: add63a89a451b742778dda1d6d313d58f675a642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918765"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="9b7f6-103">Тип ресурса sharingDetail</span><span class="sxs-lookup"><span data-stu-id="9b7f6-103">sharingDetail resource type</span></span>

> <span data-ttu-id="9b7f6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b7f6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b7f6-106">Сложный тип, содержащий свойства [общих](insights-shared.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="9b7f6-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b7f6-107">JSON representation</span></span>
<span data-ttu-id="9b7f6-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-108">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="9b7f6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b7f6-109">Properties</span></span>

| <span data-ttu-id="9b7f6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b7f6-110">Property</span></span>              | <span data-ttu-id="9b7f6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9b7f6-111">Type</span></span>          | <span data-ttu-id="9b7f6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9b7f6-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="9b7f6-113">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b7f6-113">sharedDateTime</span></span>        | <span data-ttu-id="9b7f6-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b7f6-114">DateTimeOffset</span></span>| <span data-ttu-id="9b7f6-115">Дата и время последнего общий файл.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-115">The date and time the file was last shared.</span></span> <span data-ttu-id="9b7f6-116">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9b7f6-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9b7f6-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="9b7f6-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-118">Read-only.</span></span>  |
| <span data-ttu-id="9b7f6-119">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="9b7f6-119">sharingSubject</span></span>        | <span data-ttu-id="9b7f6-120">Строка</span><span class="sxs-lookup"><span data-stu-id="9b7f6-120">String</span></span>          | <span data-ttu-id="9b7f6-121">Тема, с которым предоставлен общий доступ в документе.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-121">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="9b7f6-122">sharingType</span><span class="sxs-lookup"><span data-stu-id="9b7f6-122">sharingType</span></span>             | <span data-ttu-id="9b7f6-123">Строка</span><span class="sxs-lookup"><span data-stu-id="9b7f6-123">String</span></span>        | <span data-ttu-id="9b7f6-124">Определяет способ документ предоставлен общий доступ, может быть «Ссылка», «Вложения», «Группа», «Сайт».</span><span class="sxs-lookup"><span data-stu-id="9b7f6-124">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="9b7f6-125">sharedBy</span><span class="sxs-lookup"><span data-stu-id="9b7f6-125">sharedBy</span></span>                | [<span data-ttu-id="9b7f6-126">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="9b7f6-126">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="9b7f6-127">Пользователь, общих документов.</span><span class="sxs-lookup"><span data-stu-id="9b7f6-127">The user who shared the document.</span></span>  |
| <span data-ttu-id="9b7f6-128">sharingReference</span><span class="sxs-lookup"><span data-stu-id="9b7f6-128">sharingReference</span></span>        | [<span data-ttu-id="9b7f6-129">resourceReference</span><span class="sxs-lookup"><span data-stu-id="9b7f6-129">resourceReference</span></span>](insights-resourcereference.md)      |  |
