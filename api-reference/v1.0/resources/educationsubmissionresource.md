---
title: тип ресурсов educationSubmissionResource
description: Оболочка вокруг ресурса для использования в отправке.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d370e930e69e4dff93cbd22efb3104a9511cf880
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912620"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="74d03-103">тип ресурсов educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="74d03-103">educationSubmissionResource resource type</span></span>

<span data-ttu-id="74d03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74d03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74d03-105">Оболочка вокруг ресурса для использования в отправке.</span><span class="sxs-lookup"><span data-stu-id="74d03-105">A wrapper around a resource for use on a submission.</span></span> 

<span data-ttu-id="74d03-106">Обертка добавляет указатель на ресурс назначения, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="74d03-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="74d03-107">Методы</span><span class="sxs-lookup"><span data-stu-id="74d03-107">Methods</span></span>

| <span data-ttu-id="74d03-108">Метод</span><span class="sxs-lookup"><span data-stu-id="74d03-108">Method</span></span>           | <span data-ttu-id="74d03-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74d03-109">Return Type</span></span>    |<span data-ttu-id="74d03-110">Описание</span><span class="sxs-lookup"><span data-stu-id="74d03-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74d03-111">Get educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="74d03-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="74d03-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="74d03-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="74d03-113">Чтение свойств и связей объекта **educationSubmissionResource.**</span><span class="sxs-lookup"><span data-stu-id="74d03-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="74d03-114">Удаление</span><span class="sxs-lookup"><span data-stu-id="74d03-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="74d03-115">Нет</span><span class="sxs-lookup"><span data-stu-id="74d03-115">None</span></span> |<span data-ttu-id="74d03-116">Удаление **объекта educationSubmissionResource.**</span><span class="sxs-lookup"><span data-stu-id="74d03-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="74d03-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="74d03-117">Properties</span></span>
| <span data-ttu-id="74d03-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="74d03-118">Property</span></span>     | <span data-ttu-id="74d03-119">Тип</span><span class="sxs-lookup"><span data-stu-id="74d03-119">Type</span></span>   |<span data-ttu-id="74d03-120">Описание</span><span class="sxs-lookup"><span data-stu-id="74d03-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74d03-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="74d03-121">assignmentResourceUrl</span></span>|<span data-ttu-id="74d03-122">String</span><span class="sxs-lookup"><span data-stu-id="74d03-122">String</span></span>|<span data-ttu-id="74d03-123">Указатель на назначение, с которого был скопирован этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="74d03-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="74d03-124">Если это null, студент загрузил ресурс.</span><span class="sxs-lookup"><span data-stu-id="74d03-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="74d03-125">id</span><span class="sxs-lookup"><span data-stu-id="74d03-125">id</span></span>|<span data-ttu-id="74d03-126">String</span><span class="sxs-lookup"><span data-stu-id="74d03-126">String</span></span>| <span data-ttu-id="74d03-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74d03-127">Read-only.</span></span>|
|<span data-ttu-id="74d03-128">resource</span><span class="sxs-lookup"><span data-stu-id="74d03-128">resource</span></span>|[<span data-ttu-id="74d03-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="74d03-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="74d03-130">Объект Resource.</span><span class="sxs-lookup"><span data-stu-id="74d03-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74d03-131">Связи</span><span class="sxs-lookup"><span data-stu-id="74d03-131">Relationships</span></span>
<span data-ttu-id="74d03-132">Нет</span><span class="sxs-lookup"><span data-stu-id="74d03-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="74d03-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74d03-133">JSON representation</span></span>

<span data-ttu-id="74d03-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74d03-134">The following is a JSON representation of the resource.</span></span>

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


