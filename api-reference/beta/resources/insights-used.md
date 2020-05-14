---
title: Тип ресурса Усединсигхт
description: Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или изменил.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4c1d159ecb9750e7ad531f19f61d8ebbb462dbcc
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2020
ms.locfileid: "44226998"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="09e40-104">Тип ресурса Усединсигхт</span><span class="sxs-lookup"><span data-stu-id="09e40-104">usedInsight resource type</span></span>

<span data-ttu-id="09e40-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09e40-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09e40-106">Представление документов, используемых определенным пользователем.</span><span class="sxs-lookup"><span data-stu-id="09e40-106">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="09e40-107">Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или изменил.</span><span class="sxs-lookup"><span data-stu-id="09e40-107">The insights returns the most relevant documents that a user viewed or modified.</span></span> <span data-ttu-id="09e40-108">Сюда входят документы в:</span><span class="sxs-lookup"><span data-stu-id="09e40-108">This includes documents in:</span></span>

- <span data-ttu-id="09e40-109">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="09e40-109">OneDrive for Business</span></span>
- <span data-ttu-id="09e40-110">SharePoint</span><span class="sxs-lookup"><span data-stu-id="09e40-110">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="09e40-111">Методы</span><span class="sxs-lookup"><span data-stu-id="09e40-111">Methods</span></span>

| <span data-ttu-id="09e40-112">Метод</span><span class="sxs-lookup"><span data-stu-id="09e40-112">Method</span></span>       | <span data-ttu-id="09e40-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="09e40-113">Return Type</span></span>  |<span data-ttu-id="09e40-114">Описание</span><span class="sxs-lookup"><span data-stu-id="09e40-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09e40-115">Список "Использованные"</span><span class="sxs-lookup"><span data-stu-id="09e40-115">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="09e40-116">Коллекция объектов [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="09e40-116">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="09e40-117">Получение списка используемых файлов.</span><span class="sxs-lookup"><span data-stu-id="09e40-117">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="09e40-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="09e40-118">Properties</span></span>

| <span data-ttu-id="09e40-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="09e40-119">Property</span></span>              | <span data-ttu-id="09e40-120">Тип</span><span class="sxs-lookup"><span data-stu-id="09e40-120">Type</span></span>                      | <span data-ttu-id="09e40-121">Описание</span><span class="sxs-lookup"><span data-stu-id="09e40-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="09e40-122">id</span><span class="sxs-lookup"><span data-stu-id="09e40-122">id</span></span>                    | <span data-ttu-id="09e40-123">String</span><span class="sxs-lookup"><span data-stu-id="09e40-123">String</span></span>                    | <span data-ttu-id="09e40-124">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="09e40-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="09e40-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09e40-125">Read only.</span></span>        |
| <span data-ttu-id="09e40-126">ластусед</span><span class="sxs-lookup"><span data-stu-id="09e40-126">lastUsed</span></span>              | [<span data-ttu-id="09e40-127">usageDetails</span><span class="sxs-lookup"><span data-stu-id="09e40-127">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="09e40-128">Сведения о том, когда элемент был последний раз просмотрен или изменен пользователем.</span><span class="sxs-lookup"><span data-stu-id="09e40-128">Information about when the item was last viewed or modified by the user.</span></span> <span data-ttu-id="09e40-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09e40-129">Read only.</span></span>      |
| <span data-ttu-id="09e40-130">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="09e40-130">resourceVisualization</span></span> | [<span data-ttu-id="09e40-131">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="09e40-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="09e40-132">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="09e40-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="09e40-133">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="09e40-133">Read-only</span></span>      |
| <span data-ttu-id="09e40-134">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="09e40-134">resourceReference</span></span>     | [<span data-ttu-id="09e40-135">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="09e40-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="09e40-136">Справочные свойства используемого документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="09e40-136">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="09e40-137">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="09e40-137">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="09e40-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="09e40-138">Relationships</span></span>

| <span data-ttu-id="09e40-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="09e40-139">Property</span></span>      | <span data-ttu-id="09e40-140">Тип</span><span class="sxs-lookup"><span data-stu-id="09e40-140">Type</span></span>          | <span data-ttu-id="09e40-141">Описание</span><span class="sxs-lookup"><span data-stu-id="09e40-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="09e40-142">resource</span><span class="sxs-lookup"><span data-stu-id="09e40-142">resource</span></span>      | <span data-ttu-id="09e40-143">Коллекция [объектов](entity.md)</span><span class="sxs-lookup"><span data-stu-id="09e40-143">[entity](entity.md) collection</span></span>    | <span data-ttu-id="09e40-144">Используется для перехода к использованному элементу.</span><span class="sxs-lookup"><span data-stu-id="09e40-144">Used for navigating to the item that was used.</span></span> <span data-ttu-id="09e40-145">Для вложений в файл используется тип *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="09e40-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="09e40-146">Для связанных вложений используется тип *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="09e40-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09e40-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09e40-147">JSON representation</span></span>
<span data-ttu-id="09e40-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09e40-148">Here is a JSON representation of the resource</span></span>

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
