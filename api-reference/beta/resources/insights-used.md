---
title: используемый тип ресурса
description: 'Возможность получения, представляющее документы, используемые для определенного пользователя. Возвращает полезные сведения о наиболее важные документы, которые пользователь просматривать или доступны. Документы в том числе:'
ms.openlocfilehash: 3c82d268a67ef52d0ddfdad9193558080048ad6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080661"
---
# <a name="used-resource-type"></a><span data-ttu-id="530e8-105">используемый тип ресурса</span><span class="sxs-lookup"><span data-stu-id="530e8-105">used resource type</span></span>

> <span data-ttu-id="530e8-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="530e8-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="530e8-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="530e8-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="530e8-108">Возможность получения, представляющее документы, используемые для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="530e8-108">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="530e8-109">Возвращает полезные сведения о наиболее важные документы, которые пользователь просматривать или доступны.</span><span class="sxs-lookup"><span data-stu-id="530e8-109">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="530e8-110">Документы в том числе:</span><span class="sxs-lookup"><span data-stu-id="530e8-110">This includes documents in:</span></span>

- <span data-ttu-id="530e8-111">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="530e8-111">OneDrive for Business</span></span>
- <span data-ttu-id="530e8-112">SharePoint</span><span class="sxs-lookup"><span data-stu-id="530e8-112">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="530e8-113">Методы</span><span class="sxs-lookup"><span data-stu-id="530e8-113">Methods</span></span>

| <span data-ttu-id="530e8-114">Метод</span><span class="sxs-lookup"><span data-stu-id="530e8-114">Method</span></span>       | <span data-ttu-id="530e8-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="530e8-115">Return Type</span></span>  |<span data-ttu-id="530e8-116">Описание</span><span class="sxs-lookup"><span data-stu-id="530e8-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="530e8-117">Список, используемый</span><span class="sxs-lookup"><span data-stu-id="530e8-117">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="530e8-118">[insights_used](insights-used.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="530e8-118">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="530e8-119">Ознакомьтесь со списком используемые файлы.</span><span class="sxs-lookup"><span data-stu-id="530e8-119">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="530e8-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="530e8-120">Properties</span></span>

| <span data-ttu-id="530e8-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="530e8-121">Property</span></span>              | <span data-ttu-id="530e8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="530e8-122">Type</span></span>                      | <span data-ttu-id="530e8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="530e8-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="530e8-124">id</span><span class="sxs-lookup"><span data-stu-id="530e8-124">id</span></span>                    | <span data-ttu-id="530e8-125">String</span><span class="sxs-lookup"><span data-stu-id="530e8-125">String</span></span>                    | <span data-ttu-id="530e8-126">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="530e8-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="530e8-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="530e8-127">Read only.</span></span>        |
| <span data-ttu-id="530e8-128">lastUsed</span><span class="sxs-lookup"><span data-stu-id="530e8-128">lastUsed</span></span>              | [<span data-ttu-id="530e8-129">usageDetails</span><span class="sxs-lookup"><span data-stu-id="530e8-129">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="530e8-130">Сведения о последнего элемента просматривать и изменять пользователем.</span><span class="sxs-lookup"><span data-stu-id="530e8-130">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="530e8-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="530e8-131">Read only.</span></span>     |
| <span data-ttu-id="530e8-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="530e8-132">resourceVisualization</span></span> | [<span data-ttu-id="530e8-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="530e8-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="530e8-134">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="530e8-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="530e8-135">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="530e8-135">Read-only</span></span>      |
| <span data-ttu-id="530e8-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="530e8-136">resourceReference</span></span>     | [<span data-ttu-id="530e8-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="530e8-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="530e8-138">Справочник по свойства используется документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="530e8-138">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="530e8-139">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="530e8-139">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="530e8-140">Связи</span><span class="sxs-lookup"><span data-stu-id="530e8-140">Relationships</span></span>

| <span data-ttu-id="530e8-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="530e8-141">Property</span></span>      | <span data-ttu-id="530e8-142">Тип</span><span class="sxs-lookup"><span data-stu-id="530e8-142">Type</span></span>          | <span data-ttu-id="530e8-143">Описание</span><span class="sxs-lookup"><span data-stu-id="530e8-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="530e8-144">resource</span><span class="sxs-lookup"><span data-stu-id="530e8-144">resource</span></span>      | <span data-ttu-id="530e8-145">Объект</span><span class="sxs-lookup"><span data-stu-id="530e8-145">Entity</span></span>        | <span data-ttu-id="530e8-146">Используется для перехода к элементу, который использовался.</span><span class="sxs-lookup"><span data-stu-id="530e8-146">Used for navigating to the item that was used.</span></span> <span data-ttu-id="530e8-147">Для файлов вложений тип — *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="530e8-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="530e8-148">Для связанного вложения тип — *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="530e8-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="530e8-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="530e8-149">JSON representation</span></span>
<span data-ttu-id="530e8-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="530e8-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```