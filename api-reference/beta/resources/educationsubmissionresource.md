---
title: Тип ресурса Едукатионсубмиссионресаурце
description: 'Оболочка для ресурса, используемая при отправке. Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 876a490c3dfcf69eb993d1ba18868e2fc5a62fa8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500641"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="e7eb7-104">Тип ресурса Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="e7eb7-104">educationSubmissionResource resource type</span></span>

<span data-ttu-id="e7eb7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7eb7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7eb7-106">Оболочка для ресурса, используемая при отправке.</span><span class="sxs-lookup"><span data-stu-id="e7eb7-106">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="e7eb7-107">Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="e7eb7-107">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="e7eb7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e7eb7-108">Methods</span></span>

| <span data-ttu-id="e7eb7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e7eb7-109">Method</span></span>           | <span data-ttu-id="e7eb7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e7eb7-110">Return Type</span></span>    |<span data-ttu-id="e7eb7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e7eb7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7eb7-112">Получение Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="e7eb7-112">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="e7eb7-113">едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="e7eb7-113">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="e7eb7-114">Чтение свойств и связей объекта **едукатионсубмиссионресаурце** .</span><span class="sxs-lookup"><span data-stu-id="e7eb7-114">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|<span data-ttu-id="e7eb7-115">[удаление](../api/educationsubmissionresource-delete.md);</span><span class="sxs-lookup"><span data-stu-id="e7eb7-115">[Delete](../api/educationsubmissionresource-delete.md)</span></span> | <span data-ttu-id="e7eb7-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e7eb7-116">None</span></span> |<span data-ttu-id="e7eb7-117">Удаление объекта **едукатионсубмиссионресаурце** .</span><span class="sxs-lookup"><span data-stu-id="e7eb7-117">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7eb7-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7eb7-118">Properties</span></span>
| <span data-ttu-id="e7eb7-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7eb7-119">Property</span></span>     | <span data-ttu-id="e7eb7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e7eb7-120">Type</span></span>   |<span data-ttu-id="e7eb7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e7eb7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7eb7-122">ассигнментресаурцеурл</span><span class="sxs-lookup"><span data-stu-id="e7eb7-122">assignmentResourceUrl</span></span>|<span data-ttu-id="e7eb7-123">Строка</span><span class="sxs-lookup"><span data-stu-id="e7eb7-123">String</span></span>|<span data-ttu-id="e7eb7-124">Указатель на назначение, из которого был скопирован данный ресурс.</span><span class="sxs-lookup"><span data-stu-id="e7eb7-124">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="e7eb7-125">Если это значение равно null, учащийся передал ресурс.</span><span class="sxs-lookup"><span data-stu-id="e7eb7-125">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="e7eb7-126">id</span><span class="sxs-lookup"><span data-stu-id="e7eb7-126">id</span></span>|<span data-ttu-id="e7eb7-127">String</span><span class="sxs-lookup"><span data-stu-id="e7eb7-127">String</span></span>| <span data-ttu-id="e7eb7-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7eb7-128">Read-only.</span></span>|
|<span data-ttu-id="e7eb7-129">resource</span><span class="sxs-lookup"><span data-stu-id="e7eb7-129">resource</span></span>|[<span data-ttu-id="e7eb7-130">едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="e7eb7-130">educationResource</span></span>](educationresource.md)|<span data-ttu-id="e7eb7-131">Объект Resource.</span><span class="sxs-lookup"><span data-stu-id="e7eb7-131">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7eb7-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="e7eb7-132">Relationships</span></span>
<span data-ttu-id="e7eb7-133">Нет</span><span class="sxs-lookup"><span data-stu-id="e7eb7-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e7eb7-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7eb7-134">JSON representation</span></span>

<span data-ttu-id="e7eb7-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7eb7-135">The following is a JSON representation of the resource.</span></span>

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
