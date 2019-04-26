---
title: Тип ресурса Едукатионсубмиссионресаурце
description: 'Оболочка для ресурса, используемая при отправке. Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b96607a0d37a3ec8af0f6ff0bad61215d6e9008c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340597"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="065ba-104">Тип ресурса Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="065ba-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="065ba-105">Оболочка для ресурса, используемая при отправке.</span><span class="sxs-lookup"><span data-stu-id="065ba-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="065ba-106">Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="065ba-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="065ba-107">Методы</span><span class="sxs-lookup"><span data-stu-id="065ba-107">Methods</span></span>

| <span data-ttu-id="065ba-108">Метод</span><span class="sxs-lookup"><span data-stu-id="065ba-108">Method</span></span>           | <span data-ttu-id="065ba-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="065ba-109">Return Type</span></span>    |<span data-ttu-id="065ba-110">Описание</span><span class="sxs-lookup"><span data-stu-id="065ba-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="065ba-111">Получение Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="065ba-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="065ba-112">Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="065ba-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="065ba-113">Чтение свойств и связей объекта **едукатионсубмиссионресаурце** .</span><span class="sxs-lookup"><span data-stu-id="065ba-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="065ba-114">Delete</span><span class="sxs-lookup"><span data-stu-id="065ba-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="065ba-115">Нет</span><span class="sxs-lookup"><span data-stu-id="065ba-115">None</span></span> |<span data-ttu-id="065ba-116">Удаление объекта **едукатионсубмиссионресаурце** .</span><span class="sxs-lookup"><span data-stu-id="065ba-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="065ba-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="065ba-117">Properties</span></span>
| <span data-ttu-id="065ba-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="065ba-118">Property</span></span>     | <span data-ttu-id="065ba-119">Тип</span><span class="sxs-lookup"><span data-stu-id="065ba-119">Type</span></span>   |<span data-ttu-id="065ba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="065ba-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="065ba-121">Ассигнментресаурцеурл</span><span class="sxs-lookup"><span data-stu-id="065ba-121">assignmentResourceUrl</span></span>|<span data-ttu-id="065ba-122">String</span><span class="sxs-lookup"><span data-stu-id="065ba-122">String</span></span>|<span data-ttu-id="065ba-123">Указатель на назначение, из которого был скопирован данный ресурс.</span><span class="sxs-lookup"><span data-stu-id="065ba-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="065ba-124">Если это значение равно null, учащийся передал ресурс.</span><span class="sxs-lookup"><span data-stu-id="065ba-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="065ba-125">id</span><span class="sxs-lookup"><span data-stu-id="065ba-125">id</span></span>|<span data-ttu-id="065ba-126">String</span><span class="sxs-lookup"><span data-stu-id="065ba-126">String</span></span>| <span data-ttu-id="065ba-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="065ba-127">Read-only.</span></span>|
|<span data-ttu-id="065ba-128">resource</span><span class="sxs-lookup"><span data-stu-id="065ba-128">resource</span></span>|[<span data-ttu-id="065ba-129">Едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="065ba-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="065ba-130">Объект Resource.</span><span class="sxs-lookup"><span data-stu-id="065ba-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="065ba-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="065ba-131">Relationships</span></span>
<span data-ttu-id="065ba-132">Нет</span><span class="sxs-lookup"><span data-stu-id="065ba-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="065ba-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="065ba-133">JSON representation</span></span>

<span data-ttu-id="065ba-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="065ba-134">The following is a JSON representation of the resource.</span></span>

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
