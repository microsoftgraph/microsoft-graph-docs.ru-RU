---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9dc2d50a5bc694204317f8c3332263ce5259e2fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575106"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="f6260-103">Тип ресурса resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="f6260-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6260-104">Сложный тип, содержащий свойства [officeGraphInsights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="f6260-104">Complex type containing properties of [officeGraphInsights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6260-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6260-105">JSON representation</span></span>

<span data-ttu-id="f6260-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f6260-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
```json
{
}
```

## <a name="properties"></a><span data-ttu-id="f6260-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6260-107">Properties</span></span>

| <span data-ttu-id="f6260-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6260-108">Property</span></span>              | <span data-ttu-id="f6260-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f6260-109">Type</span></span>          | <span data-ttu-id="f6260-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6260-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="f6260-111">title</span><span class="sxs-lookup"><span data-stu-id="f6260-111">title</span></span>                 | <span data-ttu-id="f6260-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f6260-112">String</span></span>        | <span data-ttu-id="f6260-113">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="f6260-113">The item's title text.</span></span>               |
| <span data-ttu-id="f6260-114">type</span><span class="sxs-lookup"><span data-stu-id="f6260-114">type</span></span>              | <span data-ttu-id="f6260-115">Строка</span><span class="sxs-lookup"><span data-stu-id="f6260-115">String</span></span>        | <span data-ttu-id="f6260-116">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="f6260-116">The item's media type.</span></span> <span data-ttu-id="f6260-117">Можно использовать для фильтрации для конкретного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="f6260-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="f6260-118">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="f6260-118">See below for supported types.</span></span> |
| <span data-ttu-id="f6260-119">Тип носителя</span><span class="sxs-lookup"><span data-stu-id="f6260-119">mediaType</span></span>             | <span data-ttu-id="f6260-120">Строка</span><span class="sxs-lookup"><span data-stu-id="f6260-120">String</span></span>        | <span data-ttu-id="f6260-121">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="f6260-121">The item's media type.</span></span> <span data-ttu-id="f6260-122">Можно использовать для фильтрации для определенного типа файлов, поддерживаемые типы Mime IANA мультимедиа на основании.</span><span class="sxs-lookup"><span data-stu-id="f6260-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="f6260-123">Обратите внимание, что не все типы Mime мультимедиа поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="f6260-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="f6260-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="f6260-124">previewImageUrl</span></span>       | <span data-ttu-id="f6260-125">Строка</span><span class="sxs-lookup"><span data-stu-id="f6260-125">String</span></span>        | <span data-ttu-id="f6260-126">URL-адрес, приводя к изображения предварительного просмотра для элемента.</span><span class="sxs-lookup"><span data-stu-id="f6260-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="f6260-127">previewText</span><span class="sxs-lookup"><span data-stu-id="f6260-127">previewText</span></span>           | <span data-ttu-id="f6260-128">Строка</span><span class="sxs-lookup"><span data-stu-id="f6260-128">String</span></span>        | <span data-ttu-id="f6260-129">Предварительная версия текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="f6260-129">A preview text for the item.</span></span> |
| <span data-ttu-id="f6260-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="f6260-130">containerWebUrl</span></span>       | <span data-ttu-id="f6260-131">Строка</span><span class="sxs-lookup"><span data-stu-id="f6260-131">String</span></span>        | <span data-ttu-id="f6260-132">Путь, приводя к папке, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="f6260-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="f6260-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="f6260-133">containerDisplayName</span></span>  | <span data-ttu-id="f6260-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f6260-134">String</span></span>        | <span data-ttu-id="f6260-135">Строка, описывающая, где хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="f6260-135">A string describing where the item is stored.</span></span> <span data-ttu-id="f6260-136">Например имя сайт SharePoint или имя пользователя, определение владельца OneDrive, хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="f6260-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="f6260-137">containerType</span><span class="sxs-lookup"><span data-stu-id="f6260-137">containerType</span></span>         | <span data-ttu-id="f6260-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f6260-138">String</span></span> | <span data-ttu-id="f6260-139">Можно использовать для фильтрации по типу контейнер, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="f6260-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="f6260-140">Например, сайта или OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="f6260-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="f6260-141">Тип значения свойств</span><span class="sxs-lookup"><span data-stu-id="f6260-141">Type property values</span></span>
-   <span data-ttu-id="f6260-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="f6260-142">PowerPoint</span></span>
-   <span data-ttu-id="f6260-143">Word</span><span class="sxs-lookup"><span data-stu-id="f6260-143">Word</span></span>
-   <span data-ttu-id="f6260-144">Excel</span><span class="sxs-lookup"><span data-stu-id="f6260-144">Excel</span></span>
-   <span data-ttu-id="f6260-145">PDF</span><span class="sxs-lookup"><span data-stu-id="f6260-145">Pdf</span></span>
-   <span data-ttu-id="f6260-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="f6260-146">OneNote</span></span>
-   <span data-ttu-id="f6260-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="f6260-147">OneNotePage</span></span>
-   <span data-ttu-id="f6260-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="f6260-148">InfoPath</span></span>
-   <span data-ttu-id="f6260-149">Visio</span><span class="sxs-lookup"><span data-stu-id="f6260-149">Visio</span></span>
-   <span data-ttu-id="f6260-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="f6260-150">Publisher</span></span>
-   <span data-ttu-id="f6260-151">Project</span><span class="sxs-lookup"><span data-stu-id="f6260-151">Project</span></span>
-   <span data-ttu-id="f6260-152">Access</span><span class="sxs-lookup"><span data-stu-id="f6260-152">Access</span></span>
-   <span data-ttu-id="f6260-153">Почта</span><span class="sxs-lookup"><span data-stu-id="f6260-153">Mail</span></span>
-   <span data-ttu-id="f6260-154">CSV</span><span class="sxs-lookup"><span data-stu-id="f6260-154">Csv</span></span>
-   <span data-ttu-id="f6260-155">Archive</span><span class="sxs-lookup"><span data-stu-id="f6260-155">Archive</span></span>
-   <span data-ttu-id="f6260-156">XPS</span><span class="sxs-lookup"><span data-stu-id="f6260-156">Xps</span></span>
-   <span data-ttu-id="f6260-157">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="f6260-157">Audio</span></span>
-   <span data-ttu-id="f6260-158">Video (видео)</span><span class="sxs-lookup"><span data-stu-id="f6260-158">Video</span></span>
-   <span data-ttu-id="f6260-159">Изображение</span><span class="sxs-lookup"><span data-stu-id="f6260-159">Image</span></span>
-   <span data-ttu-id="f6260-160">Web</span><span class="sxs-lookup"><span data-stu-id="f6260-160">Web</span></span>
-   <span data-ttu-id="f6260-161">Текст</span><span class="sxs-lookup"><span data-stu-id="f6260-161">Text</span></span>
-   <span data-ttu-id="f6260-162">Xml</span><span class="sxs-lookup"><span data-stu-id="f6260-162">Xml</span></span>
-   <span data-ttu-id="f6260-163">Story</span><span class="sxs-lookup"><span data-stu-id="f6260-163">Story</span></span>
-   <span data-ttu-id="f6260-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="f6260-164">ExternalContent</span></span>
-   <span data-ttu-id="f6260-165">Folder</span><span class="sxs-lookup"><span data-stu-id="f6260-165">Folder</span></span>
-   <span data-ttu-id="f6260-166">Other</span><span class="sxs-lookup"><span data-stu-id="f6260-166">Other</span></span>

<span data-ttu-id="f6260-167">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="f6260-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="f6260-168">значения свойств containerType</span><span class="sxs-lookup"><span data-stu-id="f6260-168">containerType property values</span></span>
<span data-ttu-id="f6260-169">Поддерживаемые типы может отличаться в зависимости от контейнеров, с которых [возможность получения](insights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="f6260-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="f6260-170">Например только сведений об [общих](insights-shared.md) возвращает файлы из 'Общего банка данных», «Поле» и «GDrive».</span><span class="sxs-lookup"><span data-stu-id="f6260-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="f6260-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="f6260-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="f6260-172">Site</span><span class="sxs-lookup"><span data-stu-id="f6260-172">Site</span></span>
-   <span data-ttu-id="f6260-173">Почта</span><span class="sxs-lookup"><span data-stu-id="f6260-173">Mail</span></span>
-   <span data-ttu-id="f6260-174">Общего банка данных</span><span class="sxs-lookup"><span data-stu-id="f6260-174">DropBox</span></span>
-   <span data-ttu-id="f6260-175">Box</span><span class="sxs-lookup"><span data-stu-id="f6260-175">Box</span></span>
-   <span data-ttu-id="f6260-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="f6260-176">GDrive</span></span>

<span data-ttu-id="f6260-177">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="f6260-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
