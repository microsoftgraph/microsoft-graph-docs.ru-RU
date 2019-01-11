---
title: Тип ресурса recentNotebook
description: Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс notebook, но имеет меньше свойств.
localization_priority: Normal
ms.openlocfilehash: f2dd1ca642203cde36bb636b9cb2eb7c79344e3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833833"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="1efee-104">Тип ресурса recentNotebook</span><span class="sxs-lookup"><span data-stu-id="1efee-104">recentNotebook resource type</span></span>

> <span data-ttu-id="1efee-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1efee-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1efee-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1efee-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1efee-107">Недавно открытая записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="1efee-107">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="1efee-108">Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.</span><span class="sxs-lookup"><span data-stu-id="1efee-108">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="1efee-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1efee-109">Properties</span></span>
| <span data-ttu-id="1efee-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1efee-110">Property</span></span>     | <span data-ttu-id="1efee-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1efee-111">Type</span></span>   |<span data-ttu-id="1efee-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1efee-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1efee-113">name</span><span class="sxs-lookup"><span data-stu-id="1efee-113">name</span></span>|<span data-ttu-id="1efee-114">Строка</span><span class="sxs-lookup"><span data-stu-id="1efee-114">String</span></span>|<span data-ttu-id="1efee-115">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="1efee-115">The name of the notebook.</span></span>|
|<span data-ttu-id="1efee-116">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="1efee-116">lastAccessedTime</span></span>|<span data-ttu-id="1efee-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1efee-117">DateTimeOffset</span></span>|<span data-ttu-id="1efee-p104">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1efee-p104">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="1efee-122">links</span><span class="sxs-lookup"><span data-stu-id="1efee-122">links</span></span>|[<span data-ttu-id="1efee-123">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="1efee-123">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="1efee-124">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="1efee-124">Links for opening the notebook.</span></span> <span data-ttu-id="1efee-125">Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="1efee-125">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="1efee-126">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="1efee-126">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="1efee-127">sourceService</span><span class="sxs-lookup"><span data-stu-id="1efee-127">sourceService</span></span>|<span data-ttu-id="1efee-128">String</span><span class="sxs-lookup"><span data-stu-id="1efee-128">String</span></span>|<span data-ttu-id="1efee-129">Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).</span><span class="sxs-lookup"><span data-stu-id="1efee-129">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1efee-130">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1efee-130">JSON representation</span></span>

<span data-ttu-id="1efee-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1efee-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="1efee-132">Методы</span><span class="sxs-lookup"><span data-stu-id="1efee-132">Methods</span></span>

| <span data-ttu-id="1efee-133">Метод</span><span class="sxs-lookup"><span data-stu-id="1efee-133">Method</span></span>           | <span data-ttu-id="1efee-134">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1efee-134">Return Type</span></span>    |<span data-ttu-id="1efee-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1efee-135">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1efee-136">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="1efee-136">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="1efee-137">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="1efee-137">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="1efee-138">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="1efee-138">Get a collection of the most recently accessed notebooks for the user.</span></span> |
