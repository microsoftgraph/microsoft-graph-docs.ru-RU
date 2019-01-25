---
title: Тип ресурса Shared
description: 'Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя. Поддерживаются следующие общие файлы:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 11a6989e0130e7eedca7fff6f6cc9790d8109d84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524690"
---
# <a name="shared-resource-type"></a><span data-ttu-id="382dd-104">Тип ресурса Shared</span><span class="sxs-lookup"><span data-stu-id="382dd-104">shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="382dd-105">Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="382dd-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="382dd-106">Поддерживаются следующие общие файлы:</span><span class="sxs-lookup"><span data-stu-id="382dd-106">The following shared files are supported:</span></span>

- <span data-ttu-id="382dd-107">Приглашение файлами, вложенными непосредственно в сообщение электронной почты или встрече.</span><span class="sxs-lookup"><span data-stu-id="382dd-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="382dd-108">OneDrive для Bussiness и SharePoint современных вложения - файлов, хранящихся в OneDrive для бизнеса и SharePoint, которые пользователи совместно использовать как ссылки в сообщении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="382dd-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="382dd-109">**Примечание**: Корпорация Майкрософт в настоящее время работает на заполнение результатов API совместно с данными.</span><span class="sxs-lookup"><span data-stu-id="382dd-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="382dd-110">Возможно, некоторые данные, отсутствующие в первой недели после выпуска.</span><span class="sxs-lookup"><span data-stu-id="382dd-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="382dd-111">Методы</span><span class="sxs-lookup"><span data-stu-id="382dd-111">Methods</span></span>

| <span data-ttu-id="382dd-112">Метод</span><span class="sxs-lookup"><span data-stu-id="382dd-112">Method</span></span>       | <span data-ttu-id="382dd-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="382dd-113">Return Type</span></span>  |<span data-ttu-id="382dd-114">Описание</span><span class="sxs-lookup"><span data-stu-id="382dd-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="382dd-115">Список общих</span><span class="sxs-lookup"><span data-stu-id="382dd-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="382dd-116">[insights_shared](insights-shared.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="382dd-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="382dd-117">Получите список общих файлов.</span><span class="sxs-lookup"><span data-stu-id="382dd-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="382dd-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="382dd-118">Properties</span></span>

| <span data-ttu-id="382dd-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="382dd-119">Property</span></span>              | <span data-ttu-id="382dd-120">Тип</span><span class="sxs-lookup"><span data-stu-id="382dd-120">Type</span></span>                      | <span data-ttu-id="382dd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="382dd-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="382dd-122">id</span><span class="sxs-lookup"><span data-stu-id="382dd-122">id</span></span>                    | <span data-ttu-id="382dd-123">String</span><span class="sxs-lookup"><span data-stu-id="382dd-123">String</span></span>                    | <span data-ttu-id="382dd-124">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="382dd-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="382dd-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="382dd-125">Read only.</span></span>        |
| <span data-ttu-id="382dd-126">lastShared</span><span class="sxs-lookup"><span data-stu-id="382dd-126">lastShared</span></span>            | [<span data-ttu-id="382dd-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="382dd-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="382dd-128">Сведения об общих элементов.</span><span class="sxs-lookup"><span data-stu-id="382dd-128">Details about the shared item.</span></span> <span data-ttu-id="382dd-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="382dd-129">Read only.</span></span>        |
| <span data-ttu-id="382dd-130">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="382dd-130">resourceVisualization</span></span> | [<span data-ttu-id="382dd-131">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="382dd-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="382dd-132">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="382dd-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="382dd-133">Только чтение</span><span class="sxs-lookup"><span data-stu-id="382dd-133">Read-only</span></span>      |
| <span data-ttu-id="382dd-134">resourceReference</span><span class="sxs-lookup"><span data-stu-id="382dd-134">resourceReference</span></span>     | [<span data-ttu-id="382dd-135">resourceReference</span><span class="sxs-lookup"><span data-stu-id="382dd-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="382dd-136">Свойства ссылки общих документов, таких как URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="382dd-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="382dd-137">Только чтение</span><span class="sxs-lookup"><span data-stu-id="382dd-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="382dd-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="382dd-138">Relationships</span></span>

| <span data-ttu-id="382dd-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="382dd-139">Property</span></span>      | <span data-ttu-id="382dd-140">Тип</span><span class="sxs-lookup"><span data-stu-id="382dd-140">Type</span></span>          | <span data-ttu-id="382dd-141">Описание</span><span class="sxs-lookup"><span data-stu-id="382dd-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="382dd-142">resource</span><span class="sxs-lookup"><span data-stu-id="382dd-142">resource</span></span>      | <span data-ttu-id="382dd-143">Entity</span><span class="sxs-lookup"><span data-stu-id="382dd-143">Entity</span></span>        | <span data-ttu-id="382dd-144">Используется для перехода к элементу, предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="382dd-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="382dd-145">Для файлов вложений тип — *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="382dd-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="382dd-146">Для связанного вложения тип — *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="382dd-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="382dd-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="382dd-147">JSON representation</span></span>
<span data-ttu-id="382dd-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="382dd-148">Here is a JSON representation of the resource</span></span>

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
