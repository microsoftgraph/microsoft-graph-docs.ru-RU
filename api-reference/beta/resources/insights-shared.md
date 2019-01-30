---
title: тип общего ресурса
description: 'Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя. Поддерживаются следующие общие файлы:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 11a6989e0130e7eedca7fff6f6cc9790d8109d84
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640128"
---
# <a name="shared-resource-type"></a><span data-ttu-id="fdde0-104">тип общего ресурса</span><span class="sxs-lookup"><span data-stu-id="fdde0-104">shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdde0-105">Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fdde0-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="fdde0-106">Поддерживаются следующие общие файлы:</span><span class="sxs-lookup"><span data-stu-id="fdde0-106">The following shared files are supported:</span></span>

- <span data-ttu-id="fdde0-107">Приглашение файлами, вложенными непосредственно в сообщение электронной почты или встрече.</span><span class="sxs-lookup"><span data-stu-id="fdde0-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="fdde0-108">OneDrive для Bussiness и SharePoint современных вложения - файлов, хранящихся в OneDrive для бизнеса и SharePoint, которые пользователи совместно использовать как ссылки в сообщении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fdde0-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="fdde0-109">**Примечание**: Корпорация Майкрософт в настоящее время работает на заполнение результатов API совместно с данными.</span><span class="sxs-lookup"><span data-stu-id="fdde0-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="fdde0-110">Возможно, некоторые данные, отсутствующие в первой недели после выпуска.</span><span class="sxs-lookup"><span data-stu-id="fdde0-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="fdde0-111">Методы</span><span class="sxs-lookup"><span data-stu-id="fdde0-111">Methods</span></span>

| <span data-ttu-id="fdde0-112">Метод</span><span class="sxs-lookup"><span data-stu-id="fdde0-112">Method</span></span>       | <span data-ttu-id="fdde0-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fdde0-113">Return Type</span></span>  |<span data-ttu-id="fdde0-114">Описание</span><span class="sxs-lookup"><span data-stu-id="fdde0-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdde0-115">Список общих</span><span class="sxs-lookup"><span data-stu-id="fdde0-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="fdde0-116">[insights_shared](insights-shared.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fdde0-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="fdde0-117">Получите список общих файлов.</span><span class="sxs-lookup"><span data-stu-id="fdde0-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="fdde0-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdde0-118">Properties</span></span>

| <span data-ttu-id="fdde0-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdde0-119">Property</span></span>              | <span data-ttu-id="fdde0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fdde0-120">Type</span></span>                      | <span data-ttu-id="fdde0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fdde0-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="fdde0-122">id</span><span class="sxs-lookup"><span data-stu-id="fdde0-122">id</span></span>                    | <span data-ttu-id="fdde0-123">String</span><span class="sxs-lookup"><span data-stu-id="fdde0-123">String</span></span>                    | <span data-ttu-id="fdde0-124">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="fdde0-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="fdde0-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdde0-125">Read only.</span></span>        |
| <span data-ttu-id="fdde0-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="fdde0-126">lastShared</span></span>            | [<span data-ttu-id="fdde0-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="fdde0-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="fdde0-128">Сведения об общих элементов.</span><span class="sxs-lookup"><span data-stu-id="fdde0-128">Details about the shared item.</span></span> <span data-ttu-id="fdde0-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdde0-129">Read only.</span></span>        |
| <span data-ttu-id="fdde0-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="fdde0-130">resourceVisualization</span></span> | [<span data-ttu-id="fdde0-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="fdde0-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="fdde0-132">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="fdde0-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="fdde0-133">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="fdde0-133">Read-only</span></span>      |
| <span data-ttu-id="fdde0-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="fdde0-134">resourceReference</span></span>     | [<span data-ttu-id="fdde0-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="fdde0-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="fdde0-136">Свойства ссылки общих документов, таких как URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="fdde0-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="fdde0-137">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="fdde0-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="fdde0-138">Связи</span><span class="sxs-lookup"><span data-stu-id="fdde0-138">Relationships</span></span>

| <span data-ttu-id="fdde0-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdde0-139">Property</span></span>      | <span data-ttu-id="fdde0-140">Тип</span><span class="sxs-lookup"><span data-stu-id="fdde0-140">Type</span></span>          | <span data-ttu-id="fdde0-141">Описание</span><span class="sxs-lookup"><span data-stu-id="fdde0-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="fdde0-142">resource</span><span class="sxs-lookup"><span data-stu-id="fdde0-142">resource</span></span>      | <span data-ttu-id="fdde0-143">Entity</span><span class="sxs-lookup"><span data-stu-id="fdde0-143">Entity</span></span>        | <span data-ttu-id="fdde0-144">Используется для перехода к элементу, предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="fdde0-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="fdde0-145">Для файлов вложений тип — *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="fdde0-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="fdde0-146">Для связанного вложения тип — *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="fdde0-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fdde0-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdde0-147">JSON representation</span></span>
<span data-ttu-id="fdde0-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdde0-148">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
