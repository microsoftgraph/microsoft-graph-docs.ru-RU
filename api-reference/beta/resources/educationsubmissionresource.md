---
title: Тип ресурса Едукатионсубмиссионресаурце
description: 'Оболочка для ресурса, используемая при отправке. Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 48f4549354603346e39b5e1f6f387b207e2f14ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972485"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="33347-104">Тип ресурса Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="33347-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33347-105">Оболочка для ресурса, используемая при отправке.</span><span class="sxs-lookup"><span data-stu-id="33347-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="33347-106">Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="33347-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="33347-107">Методы</span><span class="sxs-lookup"><span data-stu-id="33347-107">Methods</span></span>

| <span data-ttu-id="33347-108">Метод</span><span class="sxs-lookup"><span data-stu-id="33347-108">Method</span></span>           | <span data-ttu-id="33347-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="33347-109">Return Type</span></span>    |<span data-ttu-id="33347-110">Описание</span><span class="sxs-lookup"><span data-stu-id="33347-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33347-111">Получение Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="33347-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="33347-112">Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="33347-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="33347-113">Чтение свойств и связей объекта **едукатионсубмиссионресаурце** .</span><span class="sxs-lookup"><span data-stu-id="33347-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="33347-114">Удаление</span><span class="sxs-lookup"><span data-stu-id="33347-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="33347-115">Нет</span><span class="sxs-lookup"><span data-stu-id="33347-115">None</span></span> |<span data-ttu-id="33347-116">Удаление объекта **едукатионсубмиссионресаурце** .</span><span class="sxs-lookup"><span data-stu-id="33347-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="33347-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="33347-117">Properties</span></span>
| <span data-ttu-id="33347-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="33347-118">Property</span></span>     | <span data-ttu-id="33347-119">Тип</span><span class="sxs-lookup"><span data-stu-id="33347-119">Type</span></span>   |<span data-ttu-id="33347-120">Описание</span><span class="sxs-lookup"><span data-stu-id="33347-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33347-121">Ассигнментресаурцеурл</span><span class="sxs-lookup"><span data-stu-id="33347-121">assignmentResourceUrl</span></span>|<span data-ttu-id="33347-122">String</span><span class="sxs-lookup"><span data-stu-id="33347-122">String</span></span>|<span data-ttu-id="33347-123">Указатель на назначение, из которого был скопирован данный ресурс.</span><span class="sxs-lookup"><span data-stu-id="33347-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="33347-124">Если это значение равно null, учащийся передал ресурс.</span><span class="sxs-lookup"><span data-stu-id="33347-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="33347-125">id</span><span class="sxs-lookup"><span data-stu-id="33347-125">id</span></span>|<span data-ttu-id="33347-126">String</span><span class="sxs-lookup"><span data-stu-id="33347-126">String</span></span>| <span data-ttu-id="33347-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33347-127">Read-only.</span></span>|
|<span data-ttu-id="33347-128">resource</span><span class="sxs-lookup"><span data-stu-id="33347-128">resource</span></span>|[<span data-ttu-id="33347-129">Едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="33347-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="33347-130">Объект Resource.</span><span class="sxs-lookup"><span data-stu-id="33347-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33347-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="33347-131">Relationships</span></span>
<span data-ttu-id="33347-132">Нет</span><span class="sxs-lookup"><span data-stu-id="33347-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="33347-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33347-133">JSON representation</span></span>

<span data-ttu-id="33347-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33347-134">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
