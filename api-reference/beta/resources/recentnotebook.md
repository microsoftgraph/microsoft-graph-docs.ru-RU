---
title: Тип ресурса recentNotebook
description: Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс notebook, но имеет меньше свойств.
localization_priority: Normal
ms.openlocfilehash: f79eed3a4b1c099959cb1c9bcc3f7a23a0393dfd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343999"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="ffbbc-104">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="ffbbc-104">recentNotebook resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffbbc-105">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="ffbbc-106">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="ffbbc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffbbc-107">Properties</span></span>
| <span data-ttu-id="ffbbc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffbbc-108">Property</span></span>     | <span data-ttu-id="ffbbc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ffbbc-109">Type</span></span>   |<span data-ttu-id="ffbbc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ffbbc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffbbc-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ffbbc-111">displayName</span></span>|<span data-ttu-id="ffbbc-112">String</span><span class="sxs-lookup"><span data-stu-id="ffbbc-112">String</span></span>|<span data-ttu-id="ffbbc-113">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-113">The name of the notebook.</span></span>|
|<span data-ttu-id="ffbbc-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="ffbbc-114">lastAccessedTime</span></span>|<span data-ttu-id="ffbbc-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffbbc-115">DateTimeOffset</span></span>|<span data-ttu-id="ffbbc-116">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-116">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="ffbbc-117">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ffbbc-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ffbbc-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ffbbc-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-119">Read-only.</span></span>|
|<span data-ttu-id="ffbbc-120">links</span><span class="sxs-lookup"><span data-stu-id="ffbbc-120">links</span></span>|[<span data-ttu-id="ffbbc-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="ffbbc-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="ffbbc-122">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-122">Links for opening the notebook.</span></span> <span data-ttu-id="ffbbc-123">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="ffbbc-124">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-124">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="ffbbc-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="ffbbc-125">sourceService</span></span>|<span data-ttu-id="ffbbc-126">String</span><span class="sxs-lookup"><span data-stu-id="ffbbc-126">String</span></span>|<span data-ttu-id="ffbbc-127">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="ffbbc-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffbbc-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffbbc-128">JSON representation</span></span>

<span data-ttu-id="ffbbc-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="ffbbc-130">Методы</span><span class="sxs-lookup"><span data-stu-id="ffbbc-130">Methods</span></span>

| <span data-ttu-id="ffbbc-131">Метод</span><span class="sxs-lookup"><span data-stu-id="ffbbc-131">Method</span></span>           | <span data-ttu-id="ffbbc-132">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ffbbc-132">Return Type</span></span>    |<span data-ttu-id="ffbbc-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ffbbc-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ffbbc-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="ffbbc-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="ffbbc-135">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="ffbbc-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="ffbbc-136">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="ffbbc-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
