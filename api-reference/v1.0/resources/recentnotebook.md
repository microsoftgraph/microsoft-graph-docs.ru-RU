---
title: Тип ресурса recentNotebook
description: Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс notebook, но имеет меньше свойств.
localization_priority: Normal
ms.openlocfilehash: fb5e7a7b75ea62bc644d19cf895666ba106d5dd9
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236659"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="eba96-104">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="eba96-104">recentNotebook resource type</span></span>

<span data-ttu-id="eba96-105">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="eba96-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="eba96-106">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="eba96-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="eba96-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eba96-107">Properties</span></span>
| <span data-ttu-id="eba96-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eba96-108">Property</span></span>     | <span data-ttu-id="eba96-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eba96-109">Type</span></span>   |<span data-ttu-id="eba96-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eba96-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eba96-111">displayName</span><span class="sxs-lookup"><span data-stu-id="eba96-111">displayName</span></span>|<span data-ttu-id="eba96-112">String</span><span class="sxs-lookup"><span data-stu-id="eba96-112">String</span></span>|<span data-ttu-id="eba96-113">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="eba96-113">The name of the notebook.</span></span>|
|<span data-ttu-id="eba96-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="eba96-114">lastAccessedTime</span></span>|<span data-ttu-id="eba96-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eba96-115">DateTimeOffset</span></span>|<span data-ttu-id="eba96-116">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="eba96-116">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="eba96-117">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eba96-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eba96-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="eba96-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="eba96-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eba96-119">Read-only.</span></span>|
|<span data-ttu-id="eba96-120">links</span><span class="sxs-lookup"><span data-stu-id="eba96-120">links</span></span>|[<span data-ttu-id="eba96-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="eba96-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="eba96-122">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="eba96-122">Links for opening the notebook.</span></span> <span data-ttu-id="eba96-123">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="eba96-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="eba96-124">`oneNoteWebURL` Ссылка открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="eba96-124">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="eba96-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="eba96-125">sourceService</span></span>|<span data-ttu-id="eba96-126">Оненотесаурцесервице</span><span class="sxs-lookup"><span data-stu-id="eba96-126">onenoteSourceService</span></span>|<span data-ttu-id="eba96-127">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="eba96-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eba96-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eba96-128">JSON representation</span></span>

<span data-ttu-id="eba96-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eba96-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="eba96-130">Методы</span><span class="sxs-lookup"><span data-stu-id="eba96-130">Methods</span></span>

| <span data-ttu-id="eba96-131">Метод</span><span class="sxs-lookup"><span data-stu-id="eba96-131">Method</span></span>           | <span data-ttu-id="eba96-132">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eba96-132">Return Type</span></span>    |<span data-ttu-id="eba96-133">Описание</span><span class="sxs-lookup"><span data-stu-id="eba96-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eba96-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="eba96-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="eba96-135">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="eba96-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="eba96-136">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="eba96-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
