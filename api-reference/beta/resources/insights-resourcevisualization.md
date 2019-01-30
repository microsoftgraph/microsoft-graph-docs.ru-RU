---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641297"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="25c31-103">Тип ресурса resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="25c31-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25c31-104">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="25c31-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="25c31-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25c31-105">JSON representation</span></span>

<span data-ttu-id="25c31-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="25c31-106">Here is a JSON representation of the resource</span></span>

```json
{
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a><span data-ttu-id="25c31-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="25c31-107">Properties</span></span>

| <span data-ttu-id="25c31-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="25c31-108">Property</span></span>              | <span data-ttu-id="25c31-109">Тип</span><span class="sxs-lookup"><span data-stu-id="25c31-109">Type</span></span>          | <span data-ttu-id="25c31-110">Описание</span><span class="sxs-lookup"><span data-stu-id="25c31-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="25c31-111">title</span><span class="sxs-lookup"><span data-stu-id="25c31-111">title</span></span>                 | <span data-ttu-id="25c31-112">String</span><span class="sxs-lookup"><span data-stu-id="25c31-112">String</span></span>        | <span data-ttu-id="25c31-113">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="25c31-113">The item's title text.</span></span>               |
| <span data-ttu-id="25c31-114">type</span><span class="sxs-lookup"><span data-stu-id="25c31-114">type</span></span>              | <span data-ttu-id="25c31-115">String</span><span class="sxs-lookup"><span data-stu-id="25c31-115">String</span></span>        | <span data-ttu-id="25c31-116">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="25c31-116">The item's media type.</span></span> <span data-ttu-id="25c31-117">Можно использовать для фильтрации для конкретного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="25c31-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="25c31-118">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="25c31-118">See below for supported types.</span></span> |
| <span data-ttu-id="25c31-119">Тип носителя</span><span class="sxs-lookup"><span data-stu-id="25c31-119">mediaType</span></span>             | <span data-ttu-id="25c31-120">String</span><span class="sxs-lookup"><span data-stu-id="25c31-120">String</span></span>        | <span data-ttu-id="25c31-121">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="25c31-121">The item's media type.</span></span> <span data-ttu-id="25c31-122">Можно использовать для фильтрации для определенного типа файлов, поддерживаемые типы Mime IANA мультимедиа на основании.</span><span class="sxs-lookup"><span data-stu-id="25c31-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="25c31-123">Обратите внимание, что не все типы Mime мультимедиа поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="25c31-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="25c31-124">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="25c31-124">previewImageUrl</span></span>       | <span data-ttu-id="25c31-125">String</span><span class="sxs-lookup"><span data-stu-id="25c31-125">String</span></span>        | <span data-ttu-id="25c31-126">URL-адрес, приводя к изображения предварительного просмотра для элемента.</span><span class="sxs-lookup"><span data-stu-id="25c31-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="25c31-127">previewText</span><span class="sxs-lookup"><span data-stu-id="25c31-127">previewText</span></span>           | <span data-ttu-id="25c31-128">String</span><span class="sxs-lookup"><span data-stu-id="25c31-128">String</span></span>        | <span data-ttu-id="25c31-129">Предварительная версия текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="25c31-129">A preview text for the item.</span></span> |
| <span data-ttu-id="25c31-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="25c31-130">containerWebUrl</span></span>       | <span data-ttu-id="25c31-131">String</span><span class="sxs-lookup"><span data-stu-id="25c31-131">String</span></span>        | <span data-ttu-id="25c31-132">Путь, приводя к папке, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="25c31-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="25c31-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="25c31-133">containerDisplayName</span></span>  | <span data-ttu-id="25c31-134">String</span><span class="sxs-lookup"><span data-stu-id="25c31-134">String</span></span>        | <span data-ttu-id="25c31-135">Строка, описывающая, где хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="25c31-135">A string describing where the item is stored.</span></span> <span data-ttu-id="25c31-136">Например имя сайт SharePoint или имя пользователя, определение владельца OneDrive, хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="25c31-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="25c31-137">containerType</span><span class="sxs-lookup"><span data-stu-id="25c31-137">containerType</span></span>         | <span data-ttu-id="25c31-138">String</span><span class="sxs-lookup"><span data-stu-id="25c31-138">String</span></span> | <span data-ttu-id="25c31-139">Можно использовать для фильтрации по типу контейнер, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="25c31-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="25c31-140">Например, сайта или OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="25c31-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="25c31-141">Тип значения свойств</span><span class="sxs-lookup"><span data-stu-id="25c31-141">Type property values</span></span>
-   <span data-ttu-id="25c31-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="25c31-142">PowerPoint</span></span>
-   <span data-ttu-id="25c31-143">Word</span><span class="sxs-lookup"><span data-stu-id="25c31-143">Word</span></span>
-   <span data-ttu-id="25c31-144">Excel</span><span class="sxs-lookup"><span data-stu-id="25c31-144">Excel</span></span>
-   <span data-ttu-id="25c31-145">PDF</span><span class="sxs-lookup"><span data-stu-id="25c31-145">Pdf</span></span>
-   <span data-ttu-id="25c31-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="25c31-146">OneNote</span></span>
-   <span data-ttu-id="25c31-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="25c31-147">OneNotePage</span></span>
-   <span data-ttu-id="25c31-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="25c31-148">InfoPath</span></span>
-   <span data-ttu-id="25c31-149">Visio</span><span class="sxs-lookup"><span data-stu-id="25c31-149">Visio</span></span>
-   <span data-ttu-id="25c31-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="25c31-150">Publisher</span></span>
-   <span data-ttu-id="25c31-151">Project</span><span class="sxs-lookup"><span data-stu-id="25c31-151">Project</span></span>
-   <span data-ttu-id="25c31-152">Access</span><span class="sxs-lookup"><span data-stu-id="25c31-152">Access</span></span>
-   <span data-ttu-id="25c31-153">Почта</span><span class="sxs-lookup"><span data-stu-id="25c31-153">Mail</span></span>
-   <span data-ttu-id="25c31-154">CSV</span><span class="sxs-lookup"><span data-stu-id="25c31-154">Csv</span></span>
-   <span data-ttu-id="25c31-155">Archive</span><span class="sxs-lookup"><span data-stu-id="25c31-155">Archive</span></span>
-   <span data-ttu-id="25c31-156">XPS</span><span class="sxs-lookup"><span data-stu-id="25c31-156">Xps</span></span>
-   <span data-ttu-id="25c31-157">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="25c31-157">Audio</span></span>
-   <span data-ttu-id="25c31-158">Video (видео)</span><span class="sxs-lookup"><span data-stu-id="25c31-158">Video</span></span>
-   <span data-ttu-id="25c31-159">Изображение</span><span class="sxs-lookup"><span data-stu-id="25c31-159">Image</span></span>
-   <span data-ttu-id="25c31-160">Web</span><span class="sxs-lookup"><span data-stu-id="25c31-160">Web</span></span>
-   <span data-ttu-id="25c31-161">Текст</span><span class="sxs-lookup"><span data-stu-id="25c31-161">Text</span></span>
-   <span data-ttu-id="25c31-162">Xml</span><span class="sxs-lookup"><span data-stu-id="25c31-162">Xml</span></span>
-   <span data-ttu-id="25c31-163">Story</span><span class="sxs-lookup"><span data-stu-id="25c31-163">Story</span></span>
-   <span data-ttu-id="25c31-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="25c31-164">ExternalContent</span></span>
-   <span data-ttu-id="25c31-165">Folder</span><span class="sxs-lookup"><span data-stu-id="25c31-165">Folder</span></span>
-   <span data-ttu-id="25c31-166">Other</span><span class="sxs-lookup"><span data-stu-id="25c31-166">Other</span></span>

<span data-ttu-id="25c31-167">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="25c31-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="25c31-168">значения свойств containerType</span><span class="sxs-lookup"><span data-stu-id="25c31-168">containerType property values</span></span>
<span data-ttu-id="25c31-169">Поддерживаемые типы может отличаться в зависимости от контейнеров, с которых [возможность получения](insights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="25c31-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="25c31-170">Например только сведений об [общих](insights-shared.md) возвращает файлы из 'Общего банка данных», «Поле» и «GDrive».</span><span class="sxs-lookup"><span data-stu-id="25c31-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="25c31-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="25c31-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="25c31-172">Site</span><span class="sxs-lookup"><span data-stu-id="25c31-172">Site</span></span>
-   <span data-ttu-id="25c31-173">Почта</span><span class="sxs-lookup"><span data-stu-id="25c31-173">Mail</span></span>
-   <span data-ttu-id="25c31-174">Общего банка данных</span><span class="sxs-lookup"><span data-stu-id="25c31-174">DropBox</span></span>
-   <span data-ttu-id="25c31-175">Box</span><span class="sxs-lookup"><span data-stu-id="25c31-175">Box</span></span>
-   <span data-ttu-id="25c31-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="25c31-176">GDrive</span></span>

<span data-ttu-id="25c31-177">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="25c31-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
