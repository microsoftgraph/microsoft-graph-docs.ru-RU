---
title: Тип ресурса plannerTaskDetails
description: Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче. Каждый объект Task содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 00d1360435f38cdf22547e5f509b46c931cb50b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521645"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="4a1f6-104">Тип ресурса plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="4a1f6-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="4a1f6-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4a1f6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a1f6-106">Ресурс **plannerTaskDetails** представляет дополнительные сведения о задаче.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="4a1f6-107">Каждый объект [Task](plannertask.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="4a1f6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4a1f6-108">Methods</span></span>

| <span data-ttu-id="4a1f6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4a1f6-109">Method</span></span>           | <span data-ttu-id="4a1f6-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4a1f6-110">Return Type</span></span>    |<span data-ttu-id="4a1f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a1f6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a1f6-112">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="4a1f6-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | <span data-ttu-id="4a1f6-113">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="4a1f6-113">[plannerTaskDetails](plannertaskdetails.md)</span></span> |<span data-ttu-id="4a1f6-114">Чтение свойств и связей объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="4a1f6-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|<span data-ttu-id="4a1f6-115">[обновление](../api/plannertaskdetails-update.md).</span><span class="sxs-lookup"><span data-stu-id="4a1f6-115">[Update](../api/plannertaskdetails-update.md)</span></span> | <span data-ttu-id="4a1f6-116">[plannerTaskDetails](plannertaskdetails.md);</span><span class="sxs-lookup"><span data-stu-id="4a1f6-116">[plannerTaskDetails](plannertaskdetails.md)</span></span>    |<span data-ttu-id="4a1f6-117">Обновление объекта **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="4a1f6-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4a1f6-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a1f6-118">Properties</span></span>
| <span data-ttu-id="4a1f6-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a1f6-119">Property</span></span>     | <span data-ttu-id="4a1f6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4a1f6-120">Type</span></span>   |<span data-ttu-id="4a1f6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4a1f6-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a1f6-122">checklist</span><span class="sxs-lookup"><span data-stu-id="4a1f6-122">checklist</span></span>|[<span data-ttu-id="4a1f6-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="4a1f6-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="4a1f6-124">Коллекция элементов контрольного списка задачи.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="4a1f6-125">description</span><span class="sxs-lookup"><span data-stu-id="4a1f6-125">description</span></span>|<span data-ttu-id="4a1f6-126">Строка</span><span class="sxs-lookup"><span data-stu-id="4a1f6-126">String</span></span>|<span data-ttu-id="4a1f6-127">Описание задачи.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-127">Description of the task</span></span>|
|<span data-ttu-id="4a1f6-128">id</span><span class="sxs-lookup"><span data-stu-id="4a1f6-128">id</span></span>|<span data-ttu-id="4a1f6-129">String</span><span class="sxs-lookup"><span data-stu-id="4a1f6-129">String</span></span>| <span data-ttu-id="4a1f6-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-130">Read-only.</span></span> <span data-ttu-id="4a1f6-131">Идентификатор сведений о задаче.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-131">ID of the task details.</span></span> <span data-ttu-id="4a1f6-132">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="4a1f6-133">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-133">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="4a1f6-134">previewType</span><span class="sxs-lookup"><span data-stu-id="4a1f6-134">previewType</span></span>|<span data-ttu-id="4a1f6-135">string</span><span class="sxs-lookup"><span data-stu-id="4a1f6-135">string</span></span>|<span data-ttu-id="4a1f6-p104">Устанавливает тип эскиза задачи. Возможные значения: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Если установлено значение `automatic`, отображаемый эскиз выбирается приложением, просматривающим задачу.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="4a1f6-139">references</span><span class="sxs-lookup"><span data-stu-id="4a1f6-139">references</span></span>|[<span data-ttu-id="4a1f6-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="4a1f6-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="4a1f6-141">Коллекция ссылок на задачу.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a1f6-142">Связи</span><span class="sxs-lookup"><span data-stu-id="4a1f6-142">Relationships</span></span>
<span data-ttu-id="4a1f6-143">Нет</span><span class="sxs-lookup"><span data-stu-id="4a1f6-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4a1f6-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a1f6-144">JSON representation</span></span>
<span data-ttu-id="4a1f6-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a1f6-145">Here is a JSON representation of the resource.</span></span>

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
