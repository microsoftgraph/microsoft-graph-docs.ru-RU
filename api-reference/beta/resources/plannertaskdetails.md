---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. Каждый объект Task содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: df870a8512536b0e29a923a52c62a2b779a180e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064017"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="98c6c-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="98c6c-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="98c6c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98c6c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98c6c-106">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="98c6c-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="98c6c-107">Каждый объект [Task](plannertask.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="98c6c-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="98c6c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="98c6c-108">Methods</span></span>

| <span data-ttu-id="98c6c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="98c6c-109">Method</span></span>           | <span data-ttu-id="98c6c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98c6c-110">Return Type</span></span>    |<span data-ttu-id="98c6c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98c6c-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98c6c-112">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="98c6c-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | <span data-ttu-id="98c6c-113">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="98c6c-113">[plannerTaskDetails](plannertaskdetails.md)</span></span> |<span data-ttu-id="98c6c-114">Чтение свойств и связей объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="98c6c-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="98c6c-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="98c6c-115">Update</span></span>](../api/plannertaskdetails-update.md) | <span data-ttu-id="98c6c-116">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="98c6c-116">[plannerTaskDetails](plannertaskdetails.md)</span></span>    |<span data-ttu-id="98c6c-117">Обновление объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="98c6c-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="98c6c-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="98c6c-118">Properties</span></span>
| <span data-ttu-id="98c6c-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="98c6c-119">Property</span></span>     | <span data-ttu-id="98c6c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="98c6c-120">Type</span></span>   |<span data-ttu-id="98c6c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="98c6c-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98c6c-122">checklist</span><span class="sxs-lookup"><span data-stu-id="98c6c-122">checklist</span></span>|[<span data-ttu-id="98c6c-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="98c6c-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="98c6c-124">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="98c6c-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="98c6c-125">description</span><span class="sxs-lookup"><span data-stu-id="98c6c-125">description</span></span>|<span data-ttu-id="98c6c-126">String</span><span class="sxs-lookup"><span data-stu-id="98c6c-126">String</span></span>|<span data-ttu-id="98c6c-127">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="98c6c-127">Description of the task</span></span>|
|<span data-ttu-id="98c6c-128">id</span><span class="sxs-lookup"><span data-stu-id="98c6c-128">id</span></span>|<span data-ttu-id="98c6c-129">String</span><span class="sxs-lookup"><span data-stu-id="98c6c-129">String</span></span>| <span data-ttu-id="98c6c-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98c6c-130">Read-only.</span></span> <span data-ttu-id="98c6c-131">Идентификатор сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="98c6c-131">ID of the task details.</span></span> <span data-ttu-id="98c6c-132">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="98c6c-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="98c6c-133">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="98c6c-133">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="98c6c-134">previewType</span><span class="sxs-lookup"><span data-stu-id="98c6c-134">previewType</span></span>|<span data-ttu-id="98c6c-135">string</span><span class="sxs-lookup"><span data-stu-id="98c6c-135">string</span></span>|<span data-ttu-id="98c6c-p104">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="98c6c-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="98c6c-139">references</span><span class="sxs-lookup"><span data-stu-id="98c6c-139">references</span></span>|[<span data-ttu-id="98c6c-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="98c6c-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="98c6c-141">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="98c6c-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98c6c-142">Связи</span><span class="sxs-lookup"><span data-stu-id="98c6c-142">Relationships</span></span>
<span data-ttu-id="98c6c-143">Нет</span><span class="sxs-lookup"><span data-stu-id="98c6c-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="98c6c-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98c6c-144">JSON representation</span></span>
<span data-ttu-id="98c6c-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98c6c-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


