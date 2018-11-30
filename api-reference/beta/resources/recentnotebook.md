---
title: Тип ресурса recentNotebook
description: Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс notebook, но имеет меньше свойств.
ms.openlocfilehash: c3b717fcebdc229864aefe13c6452ce5eb95fc53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078552"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="0717f-104">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="0717f-104">recentNotebook resource type</span></span>

> <span data-ttu-id="0717f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0717f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0717f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0717f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0717f-107">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="0717f-107">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="0717f-108">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="0717f-108">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="0717f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0717f-109">Properties</span></span>
| <span data-ttu-id="0717f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0717f-110">Property</span></span>     | <span data-ttu-id="0717f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0717f-111">Type</span></span>   |<span data-ttu-id="0717f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0717f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0717f-113">name</span><span class="sxs-lookup"><span data-stu-id="0717f-113">name</span></span>|<span data-ttu-id="0717f-114">String</span><span class="sxs-lookup"><span data-stu-id="0717f-114">String</span></span>|<span data-ttu-id="0717f-115">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="0717f-115">The name of the notebook.</span></span>|
|<span data-ttu-id="0717f-116">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="0717f-116">lastAccessedTime</span></span>|<span data-ttu-id="0717f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0717f-117">DateTimeOffset</span></span>|<span data-ttu-id="0717f-p104">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0717f-p104">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="0717f-122">links</span><span class="sxs-lookup"><span data-stu-id="0717f-122">links</span></span>|[<span data-ttu-id="0717f-123">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="0717f-123">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="0717f-124">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="0717f-124">Links for opening the notebook.</span></span> <span data-ttu-id="0717f-125">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="0717f-125">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="0717f-126">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="0717f-126">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="0717f-127">sourceService</span><span class="sxs-lookup"><span data-stu-id="0717f-127">sourceService</span></span>|<span data-ttu-id="0717f-128">String</span><span class="sxs-lookup"><span data-stu-id="0717f-128">String</span></span>|<span data-ttu-id="0717f-129">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="0717f-129">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0717f-130">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0717f-130">JSON representation</span></span>

<span data-ttu-id="0717f-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0717f-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}

```

## <a name="methods"></a><span data-ttu-id="0717f-132">Методы</span><span class="sxs-lookup"><span data-stu-id="0717f-132">Methods</span></span>

| <span data-ttu-id="0717f-133">Метод</span><span class="sxs-lookup"><span data-stu-id="0717f-133">Method</span></span>           | <span data-ttu-id="0717f-134">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0717f-134">Return Type</span></span>    |<span data-ttu-id="0717f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0717f-135">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0717f-136">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="0717f-136">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="0717f-137">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="0717f-137">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="0717f-138">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="0717f-138">Get a collection of the most recently accessed notebooks for the user.</span></span> |
