---
title: Тип ресурса recentNotebook
description: Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс notebook, но имеет меньше свойств.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: a35553ddb182597f1d5427418283216f962f207c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721742"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="85ab8-104">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="85ab8-104">recentNotebook resource type</span></span>

<span data-ttu-id="85ab8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85ab8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85ab8-106">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="85ab8-106">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="85ab8-107">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="85ab8-107">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="85ab8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="85ab8-108">Properties</span></span>
| <span data-ttu-id="85ab8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="85ab8-109">Property</span></span>     | <span data-ttu-id="85ab8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="85ab8-110">Type</span></span>   |<span data-ttu-id="85ab8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85ab8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85ab8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="85ab8-112">displayName</span></span>|<span data-ttu-id="85ab8-113">String</span><span class="sxs-lookup"><span data-stu-id="85ab8-113">String</span></span>|<span data-ttu-id="85ab8-114">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="85ab8-114">The name of the notebook.</span></span>|
|<span data-ttu-id="85ab8-115">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="85ab8-115">lastAccessedTime</span></span>|<span data-ttu-id="85ab8-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85ab8-116">DateTimeOffset</span></span>|<span data-ttu-id="85ab8-117">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="85ab8-117">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="85ab8-118">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="85ab8-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="85ab8-119">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="85ab8-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="85ab8-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85ab8-120">Read-only.</span></span>|
|<span data-ttu-id="85ab8-121">links</span><span class="sxs-lookup"><span data-stu-id="85ab8-121">links</span></span>|[<span data-ttu-id="85ab8-122">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="85ab8-122">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="85ab8-123">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="85ab8-123">Links for opening the notebook.</span></span> <span data-ttu-id="85ab8-124">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="85ab8-124">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="85ab8-125">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="85ab8-125">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="85ab8-126">sourceService</span><span class="sxs-lookup"><span data-stu-id="85ab8-126">sourceService</span></span>|<span data-ttu-id="85ab8-127">String</span><span class="sxs-lookup"><span data-stu-id="85ab8-127">String</span></span>|<span data-ttu-id="85ab8-128">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="85ab8-128">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85ab8-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85ab8-129">JSON representation</span></span>

<span data-ttu-id="85ab8-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85ab8-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="85ab8-131">Методы</span><span class="sxs-lookup"><span data-stu-id="85ab8-131">Methods</span></span>

| <span data-ttu-id="85ab8-132">Метод</span><span class="sxs-lookup"><span data-stu-id="85ab8-132">Method</span></span>           | <span data-ttu-id="85ab8-133">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85ab8-133">Return Type</span></span>    |<span data-ttu-id="85ab8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="85ab8-134">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85ab8-135">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="85ab8-135">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="85ab8-136">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="85ab8-136">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="85ab8-137">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="85ab8-137">Get a collection of the most recently accessed notebooks for the user.</span></span> |


