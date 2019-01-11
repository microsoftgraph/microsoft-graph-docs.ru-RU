---
title: Тип ресурса recentNotebook
description: Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс notebook, но имеет меньше свойств.
localization_priority: Normal
ms.openlocfilehash: 67c707043e5b6ca65cd72ddc323b5a484f0f2959
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889225"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="5124b-104">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="5124b-104">recentNotebook resource type</span></span>

<span data-ttu-id="5124b-105">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="5124b-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="5124b-106">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="5124b-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="5124b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5124b-107">Properties</span></span>
| <span data-ttu-id="5124b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5124b-108">Property</span></span>     | <span data-ttu-id="5124b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5124b-109">Type</span></span>   |<span data-ttu-id="5124b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5124b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5124b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5124b-111">displayName</span></span>|<span data-ttu-id="5124b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5124b-112">String</span></span>|<span data-ttu-id="5124b-113">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="5124b-113">The name of the notebook.</span></span>|
|<span data-ttu-id="5124b-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="5124b-114">lastAccessedTime</span></span>|<span data-ttu-id="5124b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5124b-115">DateTimeOffset</span></span>|<span data-ttu-id="5124b-p103">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5124b-p103">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="5124b-120">links</span><span class="sxs-lookup"><span data-stu-id="5124b-120">links</span></span>|[<span data-ttu-id="5124b-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="5124b-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="5124b-122">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="5124b-122">Links for opening the notebook.</span></span> <span data-ttu-id="5124b-123">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="5124b-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="5124b-124">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="5124b-124">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="5124b-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="5124b-125">sourceService</span></span>|<span data-ttu-id="5124b-126">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="5124b-126">onenoteSourceService</span></span>|<span data-ttu-id="5124b-127">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="5124b-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5124b-128">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5124b-128">JSON representation</span></span>

<span data-ttu-id="5124b-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5124b-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="5124b-130">Методы</span><span class="sxs-lookup"><span data-stu-id="5124b-130">Methods</span></span>

| <span data-ttu-id="5124b-131">Метод</span><span class="sxs-lookup"><span data-stu-id="5124b-131">Method</span></span>           | <span data-ttu-id="5124b-132">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5124b-132">Return Type</span></span>    |<span data-ttu-id="5124b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5124b-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5124b-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="5124b-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="5124b-135">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="5124b-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="5124b-136">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="5124b-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
