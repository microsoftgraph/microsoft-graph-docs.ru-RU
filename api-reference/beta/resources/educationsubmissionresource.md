---
title: Тип ресурса educationSubmissionResource
description: 'Оболочку ресурсов для использования на отправку. Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.  '
author: dipakboyed
ms.openlocfilehash: bfbf2f522106f5a1e2033898cbb2702223d3e241
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361560"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="227fd-104">Тип ресурса educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="227fd-104">educationSubmissionResource resource type</span></span>

> <span data-ttu-id="227fd-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="227fd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="227fd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="227fd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="227fd-107">Оболочку ресурсов для использования на отправку.</span><span class="sxs-lookup"><span data-stu-id="227fd-107">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="227fd-108">Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.</span><span class="sxs-lookup"><span data-stu-id="227fd-108">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="227fd-109">Методы</span><span class="sxs-lookup"><span data-stu-id="227fd-109">Methods</span></span>

| <span data-ttu-id="227fd-110">Метод</span><span class="sxs-lookup"><span data-stu-id="227fd-110">Method</span></span>           | <span data-ttu-id="227fd-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="227fd-111">Return Type</span></span>    |<span data-ttu-id="227fd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="227fd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="227fd-113">Получение educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="227fd-113">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="227fd-114">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="227fd-114">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="227fd-115">Чтение свойства и связи объекта **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="227fd-115">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="227fd-116">Delete</span><span class="sxs-lookup"><span data-stu-id="227fd-116">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="227fd-117">Нет</span><span class="sxs-lookup"><span data-stu-id="227fd-117">None</span></span> |<span data-ttu-id="227fd-118">Удаление объекта **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="227fd-118">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="227fd-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="227fd-119">Properties</span></span>
| <span data-ttu-id="227fd-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="227fd-120">Property</span></span>     | <span data-ttu-id="227fd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="227fd-121">Type</span></span>   |<span data-ttu-id="227fd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="227fd-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="227fd-123">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="227fd-123">assignmentResourceUrl</span></span>|<span data-ttu-id="227fd-124">String.</span><span class="sxs-lookup"><span data-stu-id="227fd-124">String</span></span>|<span data-ttu-id="227fd-125">Указатель на назначения, с которого был скопирован этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="227fd-125">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="227fd-126">Если это значение null, студент загружаться ресурса.</span><span class="sxs-lookup"><span data-stu-id="227fd-126">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="227fd-127">id</span><span class="sxs-lookup"><span data-stu-id="227fd-127">id</span></span>|<span data-ttu-id="227fd-128">Строка</span><span class="sxs-lookup"><span data-stu-id="227fd-128">String</span></span>| <span data-ttu-id="227fd-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="227fd-129">Read-only.</span></span>|
|<span data-ttu-id="227fd-130">resource</span><span class="sxs-lookup"><span data-stu-id="227fd-130">resource</span></span>|[<span data-ttu-id="227fd-131">educationResource</span><span class="sxs-lookup"><span data-stu-id="227fd-131">educationResource</span></span>](educationresource.md)|<span data-ttu-id="227fd-132">Объект ресурса.</span><span class="sxs-lookup"><span data-stu-id="227fd-132">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="227fd-133">Связи</span><span class="sxs-lookup"><span data-stu-id="227fd-133">Relationships</span></span>
<span data-ttu-id="227fd-134">Нет</span><span class="sxs-lookup"><span data-stu-id="227fd-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="227fd-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="227fd-135">JSON representation</span></span>

<span data-ttu-id="227fd-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="227fd-136">The following is a JSON representation of the resource.</span></span>

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