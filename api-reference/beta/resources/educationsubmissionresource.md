---
title: Тип ресурса educationSubmissionResource
description: 'Оболочку ресурсов для использования на отправку. Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.  '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 8703072fccb77a2577db6ce0717647e79a47fdc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875987"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="fa6f1-104">Тип ресурса educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="fa6f1-104">educationSubmissionResource resource type</span></span>

> <span data-ttu-id="fa6f1-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa6f1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa6f1-107">Оболочку ресурсов для использования на отправку.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-107">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="fa6f1-108">Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-108">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="fa6f1-109">Методы</span><span class="sxs-lookup"><span data-stu-id="fa6f1-109">Methods</span></span>

| <span data-ttu-id="fa6f1-110">Метод</span><span class="sxs-lookup"><span data-stu-id="fa6f1-110">Method</span></span>           | <span data-ttu-id="fa6f1-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fa6f1-111">Return Type</span></span>    |<span data-ttu-id="fa6f1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fa6f1-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa6f1-113">Получение educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="fa6f1-113">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="fa6f1-114">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="fa6f1-114">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="fa6f1-115">Чтение свойства и связи объекта **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="fa6f1-115">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="fa6f1-116">Delete</span><span class="sxs-lookup"><span data-stu-id="fa6f1-116">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="fa6f1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="fa6f1-117">None</span></span> |<span data-ttu-id="fa6f1-118">Удаление объекта **educationSubmissionResource** .</span><span class="sxs-lookup"><span data-stu-id="fa6f1-118">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fa6f1-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa6f1-119">Properties</span></span>
| <span data-ttu-id="fa6f1-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa6f1-120">Property</span></span>     | <span data-ttu-id="fa6f1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fa6f1-121">Type</span></span>   |<span data-ttu-id="fa6f1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fa6f1-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa6f1-123">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="fa6f1-123">assignmentResourceUrl</span></span>|<span data-ttu-id="fa6f1-124">Строка</span><span class="sxs-lookup"><span data-stu-id="fa6f1-124">String</span></span>|<span data-ttu-id="fa6f1-125">Указатель на назначения, с которого был скопирован этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-125">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="fa6f1-126">Если это значение null, студент загружаться ресурса.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-126">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="fa6f1-127">id</span><span class="sxs-lookup"><span data-stu-id="fa6f1-127">id</span></span>|<span data-ttu-id="fa6f1-128">Строка</span><span class="sxs-lookup"><span data-stu-id="fa6f1-128">String</span></span>| <span data-ttu-id="fa6f1-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-129">Read-only.</span></span>|
|<span data-ttu-id="fa6f1-130">resource</span><span class="sxs-lookup"><span data-stu-id="fa6f1-130">resource</span></span>|[<span data-ttu-id="fa6f1-131">educationResource</span><span class="sxs-lookup"><span data-stu-id="fa6f1-131">educationResource</span></span>](educationresource.md)|<span data-ttu-id="fa6f1-132">Объект ресурса.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-132">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa6f1-133">Связи</span><span class="sxs-lookup"><span data-stu-id="fa6f1-133">Relationships</span></span>
<span data-ttu-id="fa6f1-134">Нет</span><span class="sxs-lookup"><span data-stu-id="fa6f1-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fa6f1-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa6f1-135">JSON representation</span></span>

<span data-ttu-id="fa6f1-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa6f1-136">The following is a JSON representation of the resource.</span></span>

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
