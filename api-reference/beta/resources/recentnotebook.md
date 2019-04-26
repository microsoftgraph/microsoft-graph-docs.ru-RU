---
title: Тип ресурса recentNotebook
description: Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс notebook, но имеет меньше свойств.
localization_priority: Normal
ms.openlocfilehash: d1e5ef894ec521cb2826e369ca2225168105fd9a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563421"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="25496-104">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="25496-104">recentNotebook resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25496-105">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="25496-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="25496-106">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="25496-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="25496-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="25496-107">Properties</span></span>
| <span data-ttu-id="25496-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="25496-108">Property</span></span>     | <span data-ttu-id="25496-109">Тип</span><span class="sxs-lookup"><span data-stu-id="25496-109">Type</span></span>   |<span data-ttu-id="25496-110">Описание</span><span class="sxs-lookup"><span data-stu-id="25496-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25496-111">name</span><span class="sxs-lookup"><span data-stu-id="25496-111">name</span></span>|<span data-ttu-id="25496-112">String</span><span class="sxs-lookup"><span data-stu-id="25496-112">String</span></span>|<span data-ttu-id="25496-113">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="25496-113">The name of the notebook.</span></span>|
|<span data-ttu-id="25496-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="25496-114">lastAccessedTime</span></span>|<span data-ttu-id="25496-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25496-115">DateTimeOffset</span></span>|<span data-ttu-id="25496-116">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="25496-116">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="25496-117">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="25496-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="25496-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="25496-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="25496-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25496-119">Read-only.</span></span>|
|<span data-ttu-id="25496-120">links</span><span class="sxs-lookup"><span data-stu-id="25496-120">links</span></span>|[<span data-ttu-id="25496-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="25496-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="25496-122">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="25496-122">Links for opening the notebook.</span></span> <span data-ttu-id="25496-123">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="25496-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="25496-124">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="25496-124">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="25496-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="25496-125">sourceService</span></span>|<span data-ttu-id="25496-126">String</span><span class="sxs-lookup"><span data-stu-id="25496-126">String</span></span>|<span data-ttu-id="25496-127">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="25496-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25496-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25496-128">JSON representation</span></span>

<span data-ttu-id="25496-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25496-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="25496-130">Методы</span><span class="sxs-lookup"><span data-stu-id="25496-130">Methods</span></span>

| <span data-ttu-id="25496-131">Метод</span><span class="sxs-lookup"><span data-stu-id="25496-131">Method</span></span>           | <span data-ttu-id="25496-132">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="25496-132">Return Type</span></span>    |<span data-ttu-id="25496-133">Описание</span><span class="sxs-lookup"><span data-stu-id="25496-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25496-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="25496-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="25496-135">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="25496-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="25496-136">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="25496-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/recentnotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
