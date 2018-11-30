---
title: Тип ресурса educationSubmissionResource
description: 'Оболочку ресурсов для использования на отправку. Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.  '
ms.openlocfilehash: 243d0d8683683df19f7787f7cf6298770950455f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080922"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="fa533-104">Тип ресурса educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="fa533-104">educationSubmissionResource resource type</span></span>

> <span data-ttu-id="fa533-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa533-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa533-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa533-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa533-107">Оболочку ресурсов для использования на отправку.</span><span class="sxs-lookup"><span data-stu-id="fa533-107">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="fa533-108">Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.</span><span class="sxs-lookup"><span data-stu-id="fa533-108">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="fa533-109">Методы</span><span class="sxs-lookup"><span data-stu-id="fa533-109">Methods</span></span>

| <span data-ttu-id="fa533-110">Метод</span><span class="sxs-lookup"><span data-stu-id="fa533-110">Method</span></span>           | <span data-ttu-id="fa533-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fa533-111">Return Type</span></span>    |<span data-ttu-id="fa533-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fa533-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa533-113">Получение educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="fa533-113">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="fa533-114">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="fa533-114">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="fa533-115">Чтение свойства и связи объекта **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="fa533-115">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="fa533-116">Delete</span><span class="sxs-lookup"><span data-stu-id="fa533-116">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="fa533-117">Нет</span><span class="sxs-lookup"><span data-stu-id="fa533-117">None</span></span> |<span data-ttu-id="fa533-118">Удаление объекта **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="fa533-118">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fa533-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa533-119">Properties</span></span>
| <span data-ttu-id="fa533-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa533-120">Property</span></span>     | <span data-ttu-id="fa533-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fa533-121">Type</span></span>   |<span data-ttu-id="fa533-122">Description</span><span class="sxs-lookup"><span data-stu-id="fa533-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa533-123">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="fa533-123">assignmentResourceUrl</span></span>|<span data-ttu-id="fa533-124">String</span><span class="sxs-lookup"><span data-stu-id="fa533-124">String</span></span>|<span data-ttu-id="fa533-125">Указатель на назначения, с которого был скопирован этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="fa533-125">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="fa533-126">Если это значение null, студент загружаться ресурса.</span><span class="sxs-lookup"><span data-stu-id="fa533-126">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="fa533-127">id</span><span class="sxs-lookup"><span data-stu-id="fa533-127">id</span></span>|<span data-ttu-id="fa533-128">String</span><span class="sxs-lookup"><span data-stu-id="fa533-128">String</span></span>| <span data-ttu-id="fa533-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa533-129">Read-only.</span></span>|
|<span data-ttu-id="fa533-130">resource</span><span class="sxs-lookup"><span data-stu-id="fa533-130">resource</span></span>|[<span data-ttu-id="fa533-131">educationResource</span><span class="sxs-lookup"><span data-stu-id="fa533-131">educationResource</span></span>](educationresource.md)|<span data-ttu-id="fa533-132">Объект ресурса.</span><span class="sxs-lookup"><span data-stu-id="fa533-132">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa533-133">Связи</span><span class="sxs-lookup"><span data-stu-id="fa533-133">Relationships</span></span>
<span data-ttu-id="fa533-134">Нет</span><span class="sxs-lookup"><span data-stu-id="fa533-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fa533-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa533-135">JSON representation</span></span>

<span data-ttu-id="fa533-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa533-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->