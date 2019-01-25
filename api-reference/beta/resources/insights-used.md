---
title: используемый тип ресурса
description: Возможность получения, представляющее документы, используемые для определенного пользователя. Возвращает полезные сведения о наиболее важные документы, которые пользователь просматривать или доступны.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525859"
---
# <a name="used-resource-type"></a><span data-ttu-id="23d83-104">используемый тип ресурса</span><span class="sxs-lookup"><span data-stu-id="23d83-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23d83-105">Возможность получения, представляющее документы, используемые для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="23d83-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="23d83-106">Возвращает полезные сведения о наиболее важные документы, которые пользователь просматривать или доступны.</span><span class="sxs-lookup"><span data-stu-id="23d83-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="23d83-107">Документы в том числе:</span><span class="sxs-lookup"><span data-stu-id="23d83-107">This includes documents in:</span></span>

- <span data-ttu-id="23d83-108">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="23d83-108">OneDrive for Business</span></span>
- <span data-ttu-id="23d83-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="23d83-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="23d83-110">Методы</span><span class="sxs-lookup"><span data-stu-id="23d83-110">Methods</span></span>

| <span data-ttu-id="23d83-111">Метод</span><span class="sxs-lookup"><span data-stu-id="23d83-111">Method</span></span>       | <span data-ttu-id="23d83-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="23d83-112">Return Type</span></span>  |<span data-ttu-id="23d83-113">Описание</span><span class="sxs-lookup"><span data-stu-id="23d83-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="23d83-114">Список, используемый</span><span class="sxs-lookup"><span data-stu-id="23d83-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="23d83-115">[insights_used](insights-used.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="23d83-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="23d83-116">Ознакомьтесь со списком используемые файлы.</span><span class="sxs-lookup"><span data-stu-id="23d83-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="23d83-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="23d83-117">Properties</span></span>

| <span data-ttu-id="23d83-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="23d83-118">Property</span></span>              | <span data-ttu-id="23d83-119">Тип</span><span class="sxs-lookup"><span data-stu-id="23d83-119">Type</span></span>                      | <span data-ttu-id="23d83-120">Описание</span><span class="sxs-lookup"><span data-stu-id="23d83-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="23d83-121">id</span><span class="sxs-lookup"><span data-stu-id="23d83-121">id</span></span>                    | <span data-ttu-id="23d83-122">String</span><span class="sxs-lookup"><span data-stu-id="23d83-122">String</span></span>                    | <span data-ttu-id="23d83-123">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="23d83-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="23d83-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23d83-124">Read only.</span></span>        |
| <span data-ttu-id="23d83-125">lastUsed</span><span class="sxs-lookup"><span data-stu-id="23d83-125">lastUsed</span></span>              | [<span data-ttu-id="23d83-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="23d83-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="23d83-127">Сведения о последнего элемента просматривать и изменять пользователем.</span><span class="sxs-lookup"><span data-stu-id="23d83-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="23d83-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23d83-128">Read only.</span></span>     |
| <span data-ttu-id="23d83-129">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="23d83-129">resourceVisualization</span></span> | [<span data-ttu-id="23d83-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="23d83-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="23d83-131">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="23d83-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="23d83-132">Только чтение</span><span class="sxs-lookup"><span data-stu-id="23d83-132">Read-only</span></span>      |
| <span data-ttu-id="23d83-133">resourceReference</span><span class="sxs-lookup"><span data-stu-id="23d83-133">resourceReference</span></span>     | [<span data-ttu-id="23d83-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="23d83-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="23d83-135">Справочник по свойства используется документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="23d83-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="23d83-136">Только чтение</span><span class="sxs-lookup"><span data-stu-id="23d83-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="23d83-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="23d83-137">Relationships</span></span>

| <span data-ttu-id="23d83-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="23d83-138">Property</span></span>      | <span data-ttu-id="23d83-139">Тип</span><span class="sxs-lookup"><span data-stu-id="23d83-139">Type</span></span>          | <span data-ttu-id="23d83-140">Описание</span><span class="sxs-lookup"><span data-stu-id="23d83-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="23d83-141">resource</span><span class="sxs-lookup"><span data-stu-id="23d83-141">resource</span></span>      | <span data-ttu-id="23d83-142">Entity</span><span class="sxs-lookup"><span data-stu-id="23d83-142">Entity</span></span>        | <span data-ttu-id="23d83-143">Используется для перехода к элементу, который использовался.</span><span class="sxs-lookup"><span data-stu-id="23d83-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="23d83-144">Для файлов вложений тип — *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="23d83-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="23d83-145">Для связанного вложения тип — *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="23d83-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="23d83-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23d83-146">JSON representation</span></span>
<span data-ttu-id="23d83-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23d83-147">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
