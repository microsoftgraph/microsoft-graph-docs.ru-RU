---
title: Тип ресурса Едукатионсубмиссионресаурце
description: 'Оболочка для ресурса, используемая при отправке. Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 329bab18d90412ec8cc06b12106e0be4f1b46935
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979569"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="4c7c3-104">Тип ресурса Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="4c7c3-104">educationSubmissionResource resource type</span></span>

<span data-ttu-id="4c7c3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c7c3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c7c3-106">Оболочка для ресурса, используемая при отправке.</span><span class="sxs-lookup"><span data-stu-id="4c7c3-106">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="4c7c3-107">Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="4c7c3-107">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="4c7c3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4c7c3-108">Methods</span></span>

| <span data-ttu-id="4c7c3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4c7c3-109">Method</span></span>           | <span data-ttu-id="4c7c3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4c7c3-110">Return Type</span></span>    |<span data-ttu-id="4c7c3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4c7c3-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4c7c3-112">Получение Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="4c7c3-112">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="4c7c3-113">едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="4c7c3-113">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="4c7c3-114">Чтение свойств и связей объекта **едукатионсубмиссионресаурце** .</span><span class="sxs-lookup"><span data-stu-id="4c7c3-114">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|<span data-ttu-id="4c7c3-115">[удаление](../api/educationsubmissionresource-delete.md);</span><span class="sxs-lookup"><span data-stu-id="4c7c3-115">[Delete](../api/educationsubmissionresource-delete.md)</span></span> | <span data-ttu-id="4c7c3-116">Нет</span><span class="sxs-lookup"><span data-stu-id="4c7c3-116">None</span></span> |<span data-ttu-id="4c7c3-117">Удаление объекта **едукатионсубмиссионресаурце** .</span><span class="sxs-lookup"><span data-stu-id="4c7c3-117">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4c7c3-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c7c3-118">Properties</span></span>
| <span data-ttu-id="4c7c3-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c7c3-119">Property</span></span>     | <span data-ttu-id="4c7c3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4c7c3-120">Type</span></span>   |<span data-ttu-id="4c7c3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4c7c3-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c7c3-122">ассигнментресаурцеурл</span><span class="sxs-lookup"><span data-stu-id="4c7c3-122">assignmentResourceUrl</span></span>|<span data-ttu-id="4c7c3-123">String</span><span class="sxs-lookup"><span data-stu-id="4c7c3-123">String</span></span>|<span data-ttu-id="4c7c3-124">Указатель на назначение, из которого был скопирован данный ресурс.</span><span class="sxs-lookup"><span data-stu-id="4c7c3-124">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="4c7c3-125">Если это значение равно null, учащийся передал ресурс.</span><span class="sxs-lookup"><span data-stu-id="4c7c3-125">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="4c7c3-126">id</span><span class="sxs-lookup"><span data-stu-id="4c7c3-126">id</span></span>|<span data-ttu-id="4c7c3-127">String</span><span class="sxs-lookup"><span data-stu-id="4c7c3-127">String</span></span>| <span data-ttu-id="4c7c3-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c7c3-128">Read-only.</span></span>|
|<span data-ttu-id="4c7c3-129">resource</span><span class="sxs-lookup"><span data-stu-id="4c7c3-129">resource</span></span>|[<span data-ttu-id="4c7c3-130">едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="4c7c3-130">educationResource</span></span>](educationresource.md)|<span data-ttu-id="4c7c3-131">Объект Resource.</span><span class="sxs-lookup"><span data-stu-id="4c7c3-131">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c7c3-132">Связи</span><span class="sxs-lookup"><span data-stu-id="4c7c3-132">Relationships</span></span>
<span data-ttu-id="4c7c3-133">Нет</span><span class="sxs-lookup"><span data-stu-id="4c7c3-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4c7c3-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c7c3-134">JSON representation</span></span>

<span data-ttu-id="4c7c3-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c7c3-135">The following is a JSON representation of the resource.</span></span>

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


