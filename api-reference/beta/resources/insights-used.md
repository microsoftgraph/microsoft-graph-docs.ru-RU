---
title: используемый тип ресурса
description: Возможность получения, представляющее документы, используемые для определенного пользователя. Возвращает полезные сведения о наиболее важные документы, которые пользователь просматривать или доступны.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2f8479896f8c06fdc6193cfa8c18a0c3d8293bc7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976061"
---
# <a name="used-resource-type"></a><span data-ttu-id="5f04d-104">используемый тип ресурса</span><span class="sxs-lookup"><span data-stu-id="5f04d-104">used resource type</span></span>

> <span data-ttu-id="5f04d-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5f04d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f04d-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f04d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f04d-107">Возможность получения, представляющее документы, используемые для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f04d-107">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="5f04d-108">Возвращает полезные сведения о наиболее важные документы, которые пользователь просматривать или доступны.</span><span class="sxs-lookup"><span data-stu-id="5f04d-108">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="5f04d-109">Документы в том числе:</span><span class="sxs-lookup"><span data-stu-id="5f04d-109">This includes documents in:</span></span>

- <span data-ttu-id="5f04d-110">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="5f04d-110">OneDrive for Business</span></span>
- <span data-ttu-id="5f04d-111">SharePoint</span><span class="sxs-lookup"><span data-stu-id="5f04d-111">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="5f04d-112">Методы</span><span class="sxs-lookup"><span data-stu-id="5f04d-112">Methods</span></span>

| <span data-ttu-id="5f04d-113">Метод</span><span class="sxs-lookup"><span data-stu-id="5f04d-113">Method</span></span>       | <span data-ttu-id="5f04d-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5f04d-114">Return Type</span></span>  |<span data-ttu-id="5f04d-115">Описание</span><span class="sxs-lookup"><span data-stu-id="5f04d-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f04d-116">Список, используемый</span><span class="sxs-lookup"><span data-stu-id="5f04d-116">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="5f04d-117">[insights_used](insights-used.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5f04d-117">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="5f04d-118">Ознакомьтесь со списком используемые файлы.</span><span class="sxs-lookup"><span data-stu-id="5f04d-118">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f04d-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f04d-119">Properties</span></span>

| <span data-ttu-id="5f04d-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f04d-120">Property</span></span>              | <span data-ttu-id="5f04d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5f04d-121">Type</span></span>                      | <span data-ttu-id="5f04d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5f04d-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="5f04d-123">id</span><span class="sxs-lookup"><span data-stu-id="5f04d-123">id</span></span>                    | <span data-ttu-id="5f04d-124">String</span><span class="sxs-lookup"><span data-stu-id="5f04d-124">String</span></span>                    | <span data-ttu-id="5f04d-125">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="5f04d-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="5f04d-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f04d-126">Read only.</span></span>        |
| <span data-ttu-id="5f04d-127">lastUsed</span><span class="sxs-lookup"><span data-stu-id="5f04d-127">lastUsed</span></span>              | [<span data-ttu-id="5f04d-128">usageDetails</span><span class="sxs-lookup"><span data-stu-id="5f04d-128">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="5f04d-129">Сведения о последнего элемента просматривать и изменять пользователем.</span><span class="sxs-lookup"><span data-stu-id="5f04d-129">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="5f04d-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f04d-130">Read only.</span></span>     |
| <span data-ttu-id="5f04d-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="5f04d-131">resourceVisualization</span></span> | [<span data-ttu-id="5f04d-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="5f04d-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="5f04d-133">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="5f04d-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="5f04d-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="5f04d-134">Read-only</span></span>      |
| <span data-ttu-id="5f04d-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="5f04d-135">resourceReference</span></span>     | [<span data-ttu-id="5f04d-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="5f04d-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="5f04d-137">Справочник по свойства используется документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="5f04d-137">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="5f04d-138">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="5f04d-138">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="5f04d-139">Связи</span><span class="sxs-lookup"><span data-stu-id="5f04d-139">Relationships</span></span>

| <span data-ttu-id="5f04d-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f04d-140">Property</span></span>      | <span data-ttu-id="5f04d-141">Тип</span><span class="sxs-lookup"><span data-stu-id="5f04d-141">Type</span></span>          | <span data-ttu-id="5f04d-142">Описание</span><span class="sxs-lookup"><span data-stu-id="5f04d-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="5f04d-143">resource</span><span class="sxs-lookup"><span data-stu-id="5f04d-143">resource</span></span>      | <span data-ttu-id="5f04d-144">Entity</span><span class="sxs-lookup"><span data-stu-id="5f04d-144">Entity</span></span>        | <span data-ttu-id="5f04d-145">Используется для перехода к элементу, который использовался.</span><span class="sxs-lookup"><span data-stu-id="5f04d-145">Used for navigating to the item that was used.</span></span> <span data-ttu-id="5f04d-146">Для файлов вложений тип — *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="5f04d-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="5f04d-147">Для связанного вложения тип — *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="5f04d-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f04d-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f04d-148">JSON representation</span></span>
<span data-ttu-id="5f04d-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f04d-149">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
