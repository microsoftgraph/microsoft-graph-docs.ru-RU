---
title: Тип ресурса plannerExternalReference
description: Ресурс **plannerExternalReference** представляет метаданные ссылки (вложениях, например файл, URL-адрес). Это значение пары значение свойства в объекте externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d484c22d18ffb501cccbd731fa5c3ad4788a8667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944665"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="c8e85-104">Тип ресурса plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="c8e85-104">plannerExternalReference resource type</span></span>

> <span data-ttu-id="c8e85-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8e85-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8e85-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e85-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8e85-p103">Ресурс **plannerExternalReference** представляет метаданные справочных материалов (такие вложения, как файл, URL-адрес). Это значение пар "свойство-значение" в объекте [externalReferences](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="c8e85-p103">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="c8e85-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8e85-109">Properties</span></span>
| <span data-ttu-id="c8e85-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8e85-110">Property</span></span>     | <span data-ttu-id="c8e85-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c8e85-111">Type</span></span>   |<span data-ttu-id="c8e85-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e85-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8e85-113">alias</span><span class="sxs-lookup"><span data-stu-id="c8e85-113">alias</span></span>|<span data-ttu-id="c8e85-114">String</span><span class="sxs-lookup"><span data-stu-id="c8e85-114">String</span></span>|<span data-ttu-id="c8e85-115">Псевдоним имени для описания справочных материалов.</span><span class="sxs-lookup"><span data-stu-id="c8e85-115">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="c8e85-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c8e85-116">lastModifiedBy</span></span>|[<span data-ttu-id="c8e85-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="c8e85-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="c8e85-p104">Только для чтения. Идентификатор автора последних изменений.</span><span class="sxs-lookup"><span data-stu-id="c8e85-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="c8e85-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8e85-120">lastModifiedDateTime</span></span>|<span data-ttu-id="c8e85-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8e85-121">DateTimeOffset</span></span>|<span data-ttu-id="c8e85-p105">Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c8e85-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c8e85-126">previewPriority</span><span class="sxs-lookup"><span data-stu-id="c8e85-126">previewPriority</span></span>|<span data-ttu-id="c8e85-127">String</span><span class="sxs-lookup"><span data-stu-id="c8e85-127">String</span></span>|<span data-ttu-id="c8e85-128">Позволяет задать порядок относительного приоритета, согласно которому справочные материалы будут отображаться при предварительном просмотре для задачи.</span><span class="sxs-lookup"><span data-stu-id="c8e85-128">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="c8e85-129">type</span><span class="sxs-lookup"><span data-stu-id="c8e85-129">type</span></span>|<span data-ttu-id="c8e85-130">String</span><span class="sxs-lookup"><span data-stu-id="c8e85-130">String</span></span>|<span data-ttu-id="c8e85-p106">Используется для описания типа справочных материалов. Типы: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="c8e85-p106">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8e85-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c8e85-133">JSON representation</span></span>
<span data-ttu-id="c8e85-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8e85-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
