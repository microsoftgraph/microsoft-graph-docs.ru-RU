---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550740"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="5a3aa-103">Тип ресурса ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="5a3aa-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a3aa-104">Сложный тип, содержащий свойства [аналитики](insights.md).</span><span class="sxs-lookup"><span data-stu-id="5a3aa-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a3aa-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a3aa-105">JSON representation</span></span>

<span data-ttu-id="5a3aa-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="5a3aa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a3aa-107">Properties</span></span>

| <span data-ttu-id="5a3aa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a3aa-108">Property</span></span>              | <span data-ttu-id="5a3aa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5a3aa-109">Type</span></span>          | <span data-ttu-id="5a3aa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5a3aa-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="5a3aa-111">title</span><span class="sxs-lookup"><span data-stu-id="5a3aa-111">title</span></span>                 | <span data-ttu-id="5a3aa-112">String</span><span class="sxs-lookup"><span data-stu-id="5a3aa-112">String</span></span>        | <span data-ttu-id="5a3aa-113">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-113">The item's title text.</span></span>               |
| <span data-ttu-id="5a3aa-114">type</span><span class="sxs-lookup"><span data-stu-id="5a3aa-114">type</span></span>              | <span data-ttu-id="5a3aa-115">String</span><span class="sxs-lookup"><span data-stu-id="5a3aa-115">String</span></span>        | <span data-ttu-id="5a3aa-116">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-116">The item's media type.</span></span> <span data-ttu-id="5a3aa-117">Можно использовать для фильтрации определенного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="5a3aa-118">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-118">See below for supported types.</span></span> |
| <span data-ttu-id="5a3aa-119">mediaType</span><span class="sxs-lookup"><span data-stu-id="5a3aa-119">mediaType</span></span>             | <span data-ttu-id="5a3aa-120">String</span><span class="sxs-lookup"><span data-stu-id="5a3aa-120">String</span></span>        | <span data-ttu-id="5a3aa-121">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-121">The item's media type.</span></span> <span data-ttu-id="5a3aa-122">Может использоваться для фильтрации для определенного типа файлов на основе поддерживаемых типов MIME для мультимедиа IANA.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="5a3aa-123">Обратите внимание, что поддерживаются не все типы MIME мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="5a3aa-124">Превиевимажеурл</span><span class="sxs-lookup"><span data-stu-id="5a3aa-124">previewImageUrl</span></span>       | <span data-ttu-id="5a3aa-125">String</span><span class="sxs-lookup"><span data-stu-id="5a3aa-125">String</span></span>        | <span data-ttu-id="5a3aa-126">URL-адрес, ведущая к изображению для предварительного просмотра элемента.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="5a3aa-127">previewText</span><span class="sxs-lookup"><span data-stu-id="5a3aa-127">previewText</span></span>           | <span data-ttu-id="5a3aa-128">String</span><span class="sxs-lookup"><span data-stu-id="5a3aa-128">String</span></span>        | <span data-ttu-id="5a3aa-129">Предварительный текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-129">A preview text for the item.</span></span> |
| <span data-ttu-id="5a3aa-130">Контаинервебурл</span><span class="sxs-lookup"><span data-stu-id="5a3aa-130">containerWebUrl</span></span>       | <span data-ttu-id="5a3aa-131">String</span><span class="sxs-lookup"><span data-stu-id="5a3aa-131">String</span></span>        | <span data-ttu-id="5a3aa-132">Путь, начинающийся с папки, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="5a3aa-133">Контаинердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="5a3aa-133">containerDisplayName</span></span>  | <span data-ttu-id="5a3aa-134">String</span><span class="sxs-lookup"><span data-stu-id="5a3aa-134">String</span></span>        | <span data-ttu-id="5a3aa-135">Строка, описывающая место хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-135">A string describing where the item is stored.</span></span> <span data-ttu-id="5a3aa-136">Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="5a3aa-137">Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="5a3aa-137">containerType</span></span>         | <span data-ttu-id="5a3aa-138">String</span><span class="sxs-lookup"><span data-stu-id="5a3aa-138">String</span></span> | <span data-ttu-id="5a3aa-139">Можно использовать для фильтрации по типу контейнера, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="5a3aa-140">Например, site или Онедривебусинесс.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="5a3aa-141">Ввод значений свойств</span><span class="sxs-lookup"><span data-stu-id="5a3aa-141">Type property values</span></span>
-   <span data-ttu-id="5a3aa-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="5a3aa-142">PowerPoint</span></span>
-   <span data-ttu-id="5a3aa-143">Word</span><span class="sxs-lookup"><span data-stu-id="5a3aa-143">Word</span></span>
-   <span data-ttu-id="5a3aa-144">Excel</span><span class="sxs-lookup"><span data-stu-id="5a3aa-144">Excel</span></span>
-   <span data-ttu-id="5a3aa-145">]</span><span class="sxs-lookup"><span data-stu-id="5a3aa-145">Pdf</span></span>
-   <span data-ttu-id="5a3aa-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="5a3aa-146">OneNote</span></span>
-   <span data-ttu-id="5a3aa-147">Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="5a3aa-147">OneNotePage</span></span>
-   <span data-ttu-id="5a3aa-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="5a3aa-148">InfoPath</span></span>
-   <span data-ttu-id="5a3aa-149">Visio</span><span class="sxs-lookup"><span data-stu-id="5a3aa-149">Visio</span></span>
-   <span data-ttu-id="5a3aa-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="5a3aa-150">Publisher</span></span>
-   <span data-ttu-id="5a3aa-151">Project</span><span class="sxs-lookup"><span data-stu-id="5a3aa-151">Project</span></span>
-   <span data-ttu-id="5a3aa-152">Access</span><span class="sxs-lookup"><span data-stu-id="5a3aa-152">Access</span></span>
-   <span data-ttu-id="5a3aa-153">Почта</span><span class="sxs-lookup"><span data-stu-id="5a3aa-153">Mail</span></span>
-   <span data-ttu-id="5a3aa-154">Расширения</span><span class="sxs-lookup"><span data-stu-id="5a3aa-154">Csv</span></span>
-   <span data-ttu-id="5a3aa-155">Архив</span><span class="sxs-lookup"><span data-stu-id="5a3aa-155">Archive</span></span>
-   <span data-ttu-id="5a3aa-156">Компьютеров</span><span class="sxs-lookup"><span data-stu-id="5a3aa-156">Xps</span></span>
-   <span data-ttu-id="5a3aa-157">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="5a3aa-157">Audio</span></span>
-   <span data-ttu-id="5a3aa-158">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="5a3aa-158">Video</span></span>
-   <span data-ttu-id="5a3aa-159">Изображение</span><span class="sxs-lookup"><span data-stu-id="5a3aa-159">Image</span></span>
-   <span data-ttu-id="5a3aa-160">Веб</span><span class="sxs-lookup"><span data-stu-id="5a3aa-160">Web</span></span>
-   <span data-ttu-id="5a3aa-161">Текст</span><span class="sxs-lookup"><span data-stu-id="5a3aa-161">Text</span></span>
-   <span data-ttu-id="5a3aa-162">Xml</span><span class="sxs-lookup"><span data-stu-id="5a3aa-162">Xml</span></span>
-   <span data-ttu-id="5a3aa-163">Story</span><span class="sxs-lookup"><span data-stu-id="5a3aa-163">Story</span></span>
-   <span data-ttu-id="5a3aa-164">Екстерналконтент</span><span class="sxs-lookup"><span data-stu-id="5a3aa-164">ExternalContent</span></span>
-   <span data-ttu-id="5a3aa-165">Folder</span><span class="sxs-lookup"><span data-stu-id="5a3aa-165">Folder</span></span>
-   <span data-ttu-id="5a3aa-166">Другие</span><span class="sxs-lookup"><span data-stu-id="5a3aa-166">Other</span></span>

<span data-ttu-id="5a3aa-167">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="5a3aa-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="5a3aa-168">значения свойств Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="5a3aa-168">containerType property values</span></span>
<span data-ttu-id="5a3aa-169">Поддерживаемые типы могут различаться в зависимости от контейнера, из [](insights.md) которого возвращаются файлы.</span><span class="sxs-lookup"><span data-stu-id="5a3aa-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="5a3aa-170">Например, только [Общие](insights-shared.md) сведения о файлах "Dropbox", "Box" и "гдриве".</span><span class="sxs-lookup"><span data-stu-id="5a3aa-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="5a3aa-171">Онедривебусинесс</span><span class="sxs-lookup"><span data-stu-id="5a3aa-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="5a3aa-172">Сайт</span><span class="sxs-lookup"><span data-stu-id="5a3aa-172">Site</span></span>
-   <span data-ttu-id="5a3aa-173">Почта</span><span class="sxs-lookup"><span data-stu-id="5a3aa-173">Mail</span></span>
-   <span data-ttu-id="5a3aa-174">Оставляют</span><span class="sxs-lookup"><span data-stu-id="5a3aa-174">DropBox</span></span>
-   <span data-ttu-id="5a3aa-175">Box</span><span class="sxs-lookup"><span data-stu-id="5a3aa-175">Box</span></span>
-   <span data-ttu-id="5a3aa-176">Гдриве</span><span class="sxs-lookup"><span data-stu-id="5a3aa-176">GDrive</span></span>

<span data-ttu-id="5a3aa-177">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="5a3aa-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
