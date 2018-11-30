---
title: Тип ресурса plannerExternalReference
description: Ресурс **plannerExternalReference** представляет метаданные ссылки (вложениях, например файл, URL-адрес). Это значение пары значение свойства в объекте externalReferences.
ms.openlocfilehash: ad892b5e9f9a741e7a4994c509ac704ad1ca62a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075735"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="ef7eb-104">Тип ресурса plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="ef7eb-104">plannerExternalReference resource type</span></span>

> <span data-ttu-id="ef7eb-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef7eb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef7eb-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef7eb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef7eb-p103">Ресурс **plannerExternalReference** представляет метаданные справочных материалов (такие вложения, как файл, URL-адрес). Это значение пар "свойство-значение" в объекте [externalReferences](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="ef7eb-p103">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="ef7eb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef7eb-109">Properties</span></span>
| <span data-ttu-id="ef7eb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef7eb-110">Property</span></span>     | <span data-ttu-id="ef7eb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ef7eb-111">Type</span></span>   |<span data-ttu-id="ef7eb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ef7eb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef7eb-113">alias</span><span class="sxs-lookup"><span data-stu-id="ef7eb-113">alias</span></span>|<span data-ttu-id="ef7eb-114">String</span><span class="sxs-lookup"><span data-stu-id="ef7eb-114">String</span></span>|<span data-ttu-id="ef7eb-115">Псевдоним имени для описания справочных материалов.</span><span class="sxs-lookup"><span data-stu-id="ef7eb-115">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="ef7eb-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ef7eb-116">lastModifiedBy</span></span>|[<span data-ttu-id="ef7eb-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="ef7eb-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="ef7eb-p104">Только для чтения. Идентификатор автора последних изменений.</span><span class="sxs-lookup"><span data-stu-id="ef7eb-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="ef7eb-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef7eb-120">lastModifiedDateTime</span></span>|<span data-ttu-id="ef7eb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef7eb-121">DateTimeOffset</span></span>|<span data-ttu-id="ef7eb-p105">Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ef7eb-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ef7eb-126">previewPriority</span><span class="sxs-lookup"><span data-stu-id="ef7eb-126">previewPriority</span></span>|<span data-ttu-id="ef7eb-127">String</span><span class="sxs-lookup"><span data-stu-id="ef7eb-127">String</span></span>|<span data-ttu-id="ef7eb-128">Позволяет задать порядок относительного приоритета, согласно которому справочные материалы будут отображаться при предварительном просмотре для задачи.</span><span class="sxs-lookup"><span data-stu-id="ef7eb-128">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="ef7eb-129">type</span><span class="sxs-lookup"><span data-stu-id="ef7eb-129">type</span></span>|<span data-ttu-id="ef7eb-130">String</span><span class="sxs-lookup"><span data-stu-id="ef7eb-130">String</span></span>|<span data-ttu-id="ef7eb-p106">Используется для описания типа справочных материалов. Типы: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="ef7eb-p106">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef7eb-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ef7eb-133">JSON representation</span></span>
<span data-ttu-id="ef7eb-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef7eb-134">Here is a JSON representation of the resource.</span></span>

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