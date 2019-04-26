---
title: используемый тип ресурса
description: Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551293"
---
# <a name="used-resource-type"></a><span data-ttu-id="9dde7-104">используемый тип ресурса</span><span class="sxs-lookup"><span data-stu-id="9dde7-104">used resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dde7-105">Представление документов, используемых определенным пользователем.</span><span class="sxs-lookup"><span data-stu-id="9dde7-105">An insight representing documents used by a specific user.</span></span> <span data-ttu-id="9dde7-106">Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался.</span><span class="sxs-lookup"><span data-stu-id="9dde7-106">The insights returns the most relevant documents that a user viewed or accessed.</span></span> <span data-ttu-id="9dde7-107">Сюда входят документы в:</span><span class="sxs-lookup"><span data-stu-id="9dde7-107">This includes documents in:</span></span>

- <span data-ttu-id="9dde7-108">OneDrive для бизнеса</span><span class="sxs-lookup"><span data-stu-id="9dde7-108">OneDrive for Business</span></span>
- <span data-ttu-id="9dde7-109">SharePoint</span><span class="sxs-lookup"><span data-stu-id="9dde7-109">SharePoint</span></span>

## <a name="methods"></a><span data-ttu-id="9dde7-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9dde7-110">Methods</span></span>

| <span data-ttu-id="9dde7-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9dde7-111">Method</span></span>       | <span data-ttu-id="9dde7-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9dde7-112">Return Type</span></span>  |<span data-ttu-id="9dde7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9dde7-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9dde7-114">Список "Использованные"</span><span class="sxs-lookup"><span data-stu-id="9dde7-114">List used</span></span>](../api/insights-list-used.md) |<span data-ttu-id="9dde7-115">Коллекция [инсигхтс_усед](insights-used.md)</span><span class="sxs-lookup"><span data-stu-id="9dde7-115">[insights_used](insights-used.md) collection</span></span>| <span data-ttu-id="9dde7-116">Получение списка используемых файлов.</span><span class="sxs-lookup"><span data-stu-id="9dde7-116">Get a list of used files.</span></span>|

## <a name="properties"></a><span data-ttu-id="9dde7-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dde7-117">Properties</span></span>

| <span data-ttu-id="9dde7-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dde7-118">Property</span></span>              | <span data-ttu-id="9dde7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9dde7-119">Type</span></span>                      | <span data-ttu-id="9dde7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9dde7-120">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="9dde7-121">id</span><span class="sxs-lookup"><span data-stu-id="9dde7-121">id</span></span>                    | <span data-ttu-id="9dde7-122">String</span><span class="sxs-lookup"><span data-stu-id="9dde7-122">String</span></span>                    | <span data-ttu-id="9dde7-123">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="9dde7-123">Unique identifier of the relationship.</span></span> <span data-ttu-id="9dde7-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dde7-124">Read only.</span></span>        |
| <span data-ttu-id="9dde7-125">Ластусед</span><span class="sxs-lookup"><span data-stu-id="9dde7-125">lastUsed</span></span>              | [<span data-ttu-id="9dde7-126">usageDetails</span><span class="sxs-lookup"><span data-stu-id="9dde7-126">usageDetails</span></span>](insights-usagedetails.md)              | <span data-ttu-id="9dde7-127">Сведения о том, когда элемент был последний раз просмотрен и изменен пользователем.</span><span class="sxs-lookup"><span data-stu-id="9dde7-127">Information about when the item was last viewed and modified by the user.</span></span> <span data-ttu-id="9dde7-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9dde7-128">Read only.</span></span>     |
| <span data-ttu-id="9dde7-129">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="9dde7-129">resourceVisualization</span></span> | [<span data-ttu-id="9dde7-130">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="9dde7-130">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="9dde7-131">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="9dde7-131">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="9dde7-132">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="9dde7-132">Read-only</span></span>      |
| <span data-ttu-id="9dde7-133">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="9dde7-133">resourceReference</span></span>     | [<span data-ttu-id="9dde7-134">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="9dde7-134">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="9dde7-135">Справочные свойства используемого документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="9dde7-135">Reference properties of the used document, such as the url and type of the document.</span></span> <span data-ttu-id="9dde7-136">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="9dde7-136">Read-only</span></span>     |

## <a name="relationships"></a><span data-ttu-id="9dde7-137">Связи</span><span class="sxs-lookup"><span data-stu-id="9dde7-137">Relationships</span></span>

| <span data-ttu-id="9dde7-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dde7-138">Property</span></span>      | <span data-ttu-id="9dde7-139">Тип</span><span class="sxs-lookup"><span data-stu-id="9dde7-139">Type</span></span>          | <span data-ttu-id="9dde7-140">Описание</span><span class="sxs-lookup"><span data-stu-id="9dde7-140">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="9dde7-141">resource</span><span class="sxs-lookup"><span data-stu-id="9dde7-141">resource</span></span>      | <span data-ttu-id="9dde7-142">Объект</span><span class="sxs-lookup"><span data-stu-id="9dde7-142">Entity</span></span>        | <span data-ttu-id="9dde7-143">Используется для перехода к использованному элементу.</span><span class="sxs-lookup"><span data-stu-id="9dde7-143">Used for navigating to the item that was used.</span></span> <span data-ttu-id="9dde7-144">Для вложений в файл используется тип *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="9dde7-144">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="9dde7-145">Для связанных вложений используется тип *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="9dde7-145">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9dde7-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dde7-146">JSON representation</span></span>
<span data-ttu-id="9dde7-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dde7-147">Here is a JSON representation of the resource</span></span>

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
