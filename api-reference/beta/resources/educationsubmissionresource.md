---
title: Тип ресурса educationSubmissionResource
description: 'Оболочку ресурсов для использования на отправку. Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef231de49d3871ec877c279b4e77585343e1a85e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522079"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="3ae64-104">Тип ресурса educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="3ae64-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ae64-105">Оболочку ресурсов для использования на отправку.</span><span class="sxs-lookup"><span data-stu-id="3ae64-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="3ae64-106">Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.</span><span class="sxs-lookup"><span data-stu-id="3ae64-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="3ae64-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3ae64-107">Methods</span></span>

| <span data-ttu-id="3ae64-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3ae64-108">Method</span></span>           | <span data-ttu-id="3ae64-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ae64-109">Return Type</span></span>    |<span data-ttu-id="3ae64-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3ae64-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ae64-111">Получение educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="3ae64-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="3ae64-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="3ae64-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="3ae64-113">Чтение свойства и связи объекта **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="3ae64-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="3ae64-114">Delete</span><span class="sxs-lookup"><span data-stu-id="3ae64-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="3ae64-115">Нет</span><span class="sxs-lookup"><span data-stu-id="3ae64-115">None</span></span> |<span data-ttu-id="3ae64-116">Удаление объекта **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="3ae64-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ae64-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ae64-117">Properties</span></span>
| <span data-ttu-id="3ae64-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ae64-118">Property</span></span>     | <span data-ttu-id="3ae64-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3ae64-119">Type</span></span>   |<span data-ttu-id="3ae64-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3ae64-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ae64-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="3ae64-121">assignmentResourceUrl</span></span>|<span data-ttu-id="3ae64-122">String</span><span class="sxs-lookup"><span data-stu-id="3ae64-122">String</span></span>|<span data-ttu-id="3ae64-123">Указатель на назначения, с которого был скопирован этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="3ae64-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="3ae64-124">Если это значение null, студент загружаться ресурса.</span><span class="sxs-lookup"><span data-stu-id="3ae64-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="3ae64-125">id</span><span class="sxs-lookup"><span data-stu-id="3ae64-125">id</span></span>|<span data-ttu-id="3ae64-126">String</span><span class="sxs-lookup"><span data-stu-id="3ae64-126">String</span></span>| <span data-ttu-id="3ae64-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ae64-127">Read-only.</span></span>|
|<span data-ttu-id="3ae64-128">resource</span><span class="sxs-lookup"><span data-stu-id="3ae64-128">resource</span></span>|[<span data-ttu-id="3ae64-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="3ae64-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="3ae64-130">Объект Resource</span><span class="sxs-lookup"><span data-stu-id="3ae64-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ae64-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ae64-131">Relationships</span></span>
<span data-ttu-id="3ae64-132">Нет</span><span class="sxs-lookup"><span data-stu-id="3ae64-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3ae64-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ae64-133">JSON representation</span></span>

<span data-ttu-id="3ae64-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ae64-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
