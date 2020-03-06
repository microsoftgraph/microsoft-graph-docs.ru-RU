---
title: Тип ресурса Усединсигхт
description: Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8c53ef8b8b7e431319b448f26a41ce5eba857033
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531267"
---
# <a name="usedinsight-resource-type"></a><span data-ttu-id="9bf3e-104">Тип ресурса Усединсигхт</span><span class="sxs-lookup"><span data-stu-id="9bf3e-104">usedInsight resource type</span></span>

<span data-ttu-id="9bf3e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bf3e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9bf3e-106">Представление документов, используемых определенным пользователем.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-106">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="9bf3e-107">Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-107">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="9bf3e-108">Сюда входят документы в:</span><span class="sxs-lookup"><span data-stu-id="9bf3e-108">This includes documents in:</span></span>

- <span data-ttu-id="9bf3e-109">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="9bf3e-109">OneDrive for Business</span></span>
- <span data-ttu-id="9bf3e-110">SharePoint</span><span class="sxs-lookup"><span data-stu-id="9bf3e-110">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="9bf3e-111">Методы</span><span class="sxs-lookup"><span data-stu-id="9bf3e-111">Methods</span></span>

| <span data-ttu-id="9bf3e-112">Метод</span><span class="sxs-lookup"><span data-stu-id="9bf3e-112">Method</span></span>       | <span data-ttu-id="9bf3e-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9bf3e-113">Return Type</span></span>  |<span data-ttu-id="9bf3e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9bf3e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9bf3e-115">Список "Использованные"</span><span class="sxs-lookup"><span data-stu-id="9bf3e-115">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="9bf3e-116">Коллекция объектов [usedInsight](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="9bf3e-116">[usedInsight](insights-used.md) collection</span></span>| <span data-ttu-id="9bf3e-117">Получение списка используемых файлов.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-117">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="9bf3e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bf3e-118">Properties</span></span>

| <span data-ttu-id="9bf3e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bf3e-119">Property</span></span>              | <span data-ttu-id="9bf3e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9bf3e-120">Type</span></span>                      | <span data-ttu-id="9bf3e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9bf3e-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="9bf3e-122">id</span><span class="sxs-lookup"><span data-stu-id="9bf3e-122">id</span></span>                    | <span data-ttu-id="9bf3e-123">Строка</span><span class="sxs-lookup"><span data-stu-id="9bf3e-123">String</span></span>                    | <span data-ttu-id="9bf3e-124">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="9bf3e-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-125">Read only.</span></span>        |
| <span data-ttu-id="9bf3e-126">ластусед</span><span class="sxs-lookup"><span data-stu-id="9bf3e-126">lastUsed</span></span>              | [<span data-ttu-id="9bf3e-127">usageDetails</span><span class="sxs-lookup"><span data-stu-id="9bf3e-127">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="9bf3e-128">Сведения о том, когда элемент был последний раз просмотрен и изменен пользователем.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-128">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="9bf3e-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-129">Read only.</span></span>     |
| <span data-ttu-id="9bf3e-130">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="9bf3e-130">resourceVisualization</span></span> | [<span data-ttu-id="9bf3e-131">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="9bf3e-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="9bf3e-132">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="9bf3e-133">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="9bf3e-133">Read-only</span></span>      |
| <span data-ttu-id="9bf3e-134">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="9bf3e-134">resourceReference</span></span>     | [<span data-ttu-id="9bf3e-135">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="9bf3e-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="9bf3e-136">Справочные свойства используемого документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-136">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="9bf3e-137">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="9bf3e-137">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="9bf3e-138">Связи</span><span class="sxs-lookup"><span data-stu-id="9bf3e-138">Relationships</span></span>

| <span data-ttu-id="9bf3e-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bf3e-139">Property</span></span>      | <span data-ttu-id="9bf3e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="9bf3e-140">Type</span></span>          | <span data-ttu-id="9bf3e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="9bf3e-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="9bf3e-142">resource</span><span class="sxs-lookup"><span data-stu-id="9bf3e-142">resource</span></span>      | <span data-ttu-id="9bf3e-143">Коллекция [объектов](entity.md)</span><span class="sxs-lookup"><span data-stu-id="9bf3e-143">[entity](entity.md) collection</span></span>    | <span data-ttu-id="9bf3e-144">Используется для перехода к использованному элементу.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-144">Used for navigating to the item that was used.</span></span> <span data-ttu-id="9bf3e-145">Для вложений в файл используется тип *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="9bf3e-146">Для связанных вложений используется тип *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9bf3e-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bf3e-147">JSON representation</span></span>
<span data-ttu-id="9bf3e-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bf3e-148">Here is a JSON representation of the resource</span></span>

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
