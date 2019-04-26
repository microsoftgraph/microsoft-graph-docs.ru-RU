---
title: Тип ресурса Усединсигхт
description: Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 407822dc4ff3f0536b0cbff3bf2894ad96d5d878
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333556"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="b7adb-104">Тип ресурса Усединсигхт</span><span class="sxs-lookup"><span data-stu-id="b7adb-104">usedInsight resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7adb-105">Представление документов, используемых определенным пользователем.</span><span class="sxs-lookup"><span data-stu-id="b7adb-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="b7adb-106">Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался.</span><span class="sxs-lookup"><span data-stu-id="b7adb-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="b7adb-107">Сюда входят документы в:</span><span class="sxs-lookup"><span data-stu-id="b7adb-107">This includes documents in:</span></span>

- <span data-ttu-id="b7adb-108">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="b7adb-108">OneDrive for Business</span></span>
- <span data-ttu-id="b7adb-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="b7adb-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="b7adb-110">Методы</span><span class="sxs-lookup"><span data-stu-id="b7adb-110">Methods</span></span>

| <span data-ttu-id="b7adb-111">Метод</span><span class="sxs-lookup"><span data-stu-id="b7adb-111">Method</span></span>       | <span data-ttu-id="b7adb-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b7adb-112">Return Type</span></span>  |<span data-ttu-id="b7adb-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b7adb-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b7adb-114">Список "Использованные"</span><span class="sxs-lookup"><span data-stu-id="b7adb-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="b7adb-115">Коллекция [усединсигхт](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="b7adb-115">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="b7adb-116">Получение списка используемых файлов.</span><span class="sxs-lookup"><span data-stu-id="b7adb-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7adb-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7adb-117">Properties</span></span>

| <span data-ttu-id="b7adb-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7adb-118">Property</span></span>              | <span data-ttu-id="b7adb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b7adb-119">Type</span></span>                      | <span data-ttu-id="b7adb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b7adb-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="b7adb-121">id</span><span class="sxs-lookup"><span data-stu-id="b7adb-121">id</span></span>                    | <span data-ttu-id="b7adb-122">String</span><span class="sxs-lookup"><span data-stu-id="b7adb-122">String</span></span>                    | <span data-ttu-id="b7adb-123">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="b7adb-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="b7adb-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7adb-124">Read only.</span></span>        |
| <span data-ttu-id="b7adb-125">Ластусед</span><span class="sxs-lookup"><span data-stu-id="b7adb-125">lastUsed</span></span>              | [<span data-ttu-id="b7adb-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="b7adb-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="b7adb-127">Сведения о том, когда элемент был последний раз просмотрен и изменен пользователем.</span><span class="sxs-lookup"><span data-stu-id="b7adb-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="b7adb-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b7adb-128">Read only.</span></span>     |
| <span data-ttu-id="b7adb-129">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="b7adb-129">resourceVisualization</span></span> | [<span data-ttu-id="b7adb-130">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="b7adb-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="b7adb-131">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="b7adb-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="b7adb-132">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="b7adb-132">Read-only</span></span>      |
| <span data-ttu-id="b7adb-133">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="b7adb-133">resourceReference</span></span>     | [<span data-ttu-id="b7adb-134">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="b7adb-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="b7adb-135">Справочные свойства используемого документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="b7adb-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="b7adb-136">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="b7adb-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="b7adb-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="b7adb-137">Relationships</span></span>

| <span data-ttu-id="b7adb-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7adb-138">Property</span></span>      | <span data-ttu-id="b7adb-139">Тип</span><span class="sxs-lookup"><span data-stu-id="b7adb-139">Type</span></span>          | <span data-ttu-id="b7adb-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b7adb-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="b7adb-141">resource</span><span class="sxs-lookup"><span data-stu-id="b7adb-141">resource</span></span>      | <span data-ttu-id="b7adb-142">Коллекция [объектов](entity.md)</span><span class="sxs-lookup"><span data-stu-id="b7adb-142">[entity](entity.md) collection</span></span>    | <span data-ttu-id="b7adb-143">Используется для перехода к использованному элементу.</span><span class="sxs-lookup"><span data-stu-id="b7adb-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="b7adb-144">Для вложений в файл используется тип *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="b7adb-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="b7adb-145">Для связанных вложений используется тип *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="b7adb-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b7adb-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7adb-146">JSON representation</span></span>
<span data-ttu-id="b7adb-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7adb-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```
