---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: b49ce2c0fb0c1d2ab167ffbb033bf11b0171a20f
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844493"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="c2d60-103">Тип ресурса ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="c2d60-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2d60-104">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="c2d60-104">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2d60-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2d60-105">JSON representation</span></span>

<span data-ttu-id="c2d60-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c2d60-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
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

## <a name="properties"></a><span data-ttu-id="c2d60-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2d60-107">Properties</span></span>

| <span data-ttu-id="c2d60-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d60-108">Property</span></span>              | <span data-ttu-id="c2d60-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d60-109">Type</span></span>          | <span data-ttu-id="c2d60-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d60-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="c2d60-111">title</span><span class="sxs-lookup"><span data-stu-id="c2d60-111">title</span></span>                 | <span data-ttu-id="c2d60-112">String</span><span class="sxs-lookup"><span data-stu-id="c2d60-112">String</span></span>        | <span data-ttu-id="c2d60-113">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="c2d60-113">The item's title text.</span></span>               |
| <span data-ttu-id="c2d60-114">type</span><span class="sxs-lookup"><span data-stu-id="c2d60-114">type</span></span>              | <span data-ttu-id="c2d60-115">String</span><span class="sxs-lookup"><span data-stu-id="c2d60-115">String</span></span>        | <span data-ttu-id="c2d60-116">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="c2d60-116">The item's media type.</span></span> <span data-ttu-id="c2d60-117">Можно использовать для фильтрации определенного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="c2d60-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="c2d60-118">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="c2d60-118">See below for supported types.</span></span> |
| <span data-ttu-id="c2d60-119">mediaType</span><span class="sxs-lookup"><span data-stu-id="c2d60-119">mediaType</span></span>             | <span data-ttu-id="c2d60-120">String</span><span class="sxs-lookup"><span data-stu-id="c2d60-120">String</span></span>        | <span data-ttu-id="c2d60-121">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="c2d60-121">The item's media type.</span></span> <span data-ttu-id="c2d60-122">Может использоваться для фильтрации файлов определенного типа на основе поддерживаемых типов MIME MIME для устройства IANA.</span><span class="sxs-lookup"><span data-stu-id="c2d60-122">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="c2d60-123">Обратите внимание, что поддерживаются не все типы MIME мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c2d60-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="c2d60-124">превиевимажеурл</span><span class="sxs-lookup"><span data-stu-id="c2d60-124">previewImageUrl</span></span>       | <span data-ttu-id="c2d60-125">String</span><span class="sxs-lookup"><span data-stu-id="c2d60-125">String</span></span>        | <span data-ttu-id="c2d60-126">URL-адрес, ведущая к изображению для предварительного просмотра элемента.</span><span class="sxs-lookup"><span data-stu-id="c2d60-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="c2d60-127">previewText</span><span class="sxs-lookup"><span data-stu-id="c2d60-127">previewText</span></span>           | <span data-ttu-id="c2d60-128">String</span><span class="sxs-lookup"><span data-stu-id="c2d60-128">String</span></span>        | <span data-ttu-id="c2d60-129">Предварительный текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="c2d60-129">A preview text for the item.</span></span> |
| <span data-ttu-id="c2d60-130">контаинервебурл</span><span class="sxs-lookup"><span data-stu-id="c2d60-130">containerWebUrl</span></span>       | <span data-ttu-id="c2d60-131">String</span><span class="sxs-lookup"><span data-stu-id="c2d60-131">String</span></span>        | <span data-ttu-id="c2d60-132">Путь, начинающийся с папки, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="c2d60-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="c2d60-133">контаинердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="c2d60-133">containerDisplayName</span></span>  | <span data-ttu-id="c2d60-134">String</span><span class="sxs-lookup"><span data-stu-id="c2d60-134">String</span></span>        | <span data-ttu-id="c2d60-135">Строка, описывающая место хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="c2d60-135">A string describing where the item is stored.</span></span> <span data-ttu-id="c2d60-136">Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="c2d60-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="c2d60-137">контаинертипе</span><span class="sxs-lookup"><span data-stu-id="c2d60-137">containerType</span></span>         | <span data-ttu-id="c2d60-138">String</span><span class="sxs-lookup"><span data-stu-id="c2d60-138">String</span></span> | <span data-ttu-id="c2d60-139">Можно использовать для фильтрации по типу контейнера, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="c2d60-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="c2d60-140">Например, site или Онедривебусинесс.</span><span class="sxs-lookup"><span data-stu-id="c2d60-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="c2d60-141">Ввод значений свойств</span><span class="sxs-lookup"><span data-stu-id="c2d60-141">Type property values</span></span>
-   <span data-ttu-id="c2d60-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="c2d60-142">PowerPoint</span></span>
-   <span data-ttu-id="c2d60-143">Word</span><span class="sxs-lookup"><span data-stu-id="c2d60-143">Word</span></span>
-   <span data-ttu-id="c2d60-144">Excel</span><span class="sxs-lookup"><span data-stu-id="c2d60-144">Excel</span></span>
-   <span data-ttu-id="c2d60-145">]</span><span class="sxs-lookup"><span data-stu-id="c2d60-145">Pdf</span></span>
-   <span data-ttu-id="c2d60-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="c2d60-146">OneNote</span></span>
-   <span data-ttu-id="c2d60-147">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="c2d60-147">OneNotePage</span></span>
-   <span data-ttu-id="c2d60-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="c2d60-148">InfoPath</span></span>
-   <span data-ttu-id="c2d60-149">Visio</span><span class="sxs-lookup"><span data-stu-id="c2d60-149">Visio</span></span>
-   <span data-ttu-id="c2d60-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="c2d60-150">Publisher</span></span>
-   <span data-ttu-id="c2d60-151">Project</span><span class="sxs-lookup"><span data-stu-id="c2d60-151">Project</span></span>
-   <span data-ttu-id="c2d60-152">Access</span><span class="sxs-lookup"><span data-stu-id="c2d60-152">Access</span></span>
-   <span data-ttu-id="c2d60-153">Почта</span><span class="sxs-lookup"><span data-stu-id="c2d60-153">Mail</span></span>
-   <span data-ttu-id="c2d60-154">Расширения</span><span class="sxs-lookup"><span data-stu-id="c2d60-154">Csv</span></span>
-   <span data-ttu-id="c2d60-155">Архив</span><span class="sxs-lookup"><span data-stu-id="c2d60-155">Archive</span></span>
-   <span data-ttu-id="c2d60-156">Компьютеров</span><span class="sxs-lookup"><span data-stu-id="c2d60-156">Xps</span></span>
-   <span data-ttu-id="c2d60-157">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="c2d60-157">Audio</span></span>
-   <span data-ttu-id="c2d60-158">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="c2d60-158">Video</span></span>
-   <span data-ttu-id="c2d60-159">Изображение</span><span class="sxs-lookup"><span data-stu-id="c2d60-159">Image</span></span>
-   <span data-ttu-id="c2d60-160">Web</span><span class="sxs-lookup"><span data-stu-id="c2d60-160">Web</span></span>
-   <span data-ttu-id="c2d60-161">Текст</span><span class="sxs-lookup"><span data-stu-id="c2d60-161">Text</span></span>
-   <span data-ttu-id="c2d60-162">Xml</span><span class="sxs-lookup"><span data-stu-id="c2d60-162">Xml</span></span>
-   <span data-ttu-id="c2d60-163">Story</span><span class="sxs-lookup"><span data-stu-id="c2d60-163">Story</span></span>
-   <span data-ttu-id="c2d60-164">екстерналконтент</span><span class="sxs-lookup"><span data-stu-id="c2d60-164">ExternalContent</span></span>
-   <span data-ttu-id="c2d60-165">Folder</span><span class="sxs-lookup"><span data-stu-id="c2d60-165">Folder</span></span>
-   <span data-ttu-id="c2d60-166">Other</span><span class="sxs-lookup"><span data-stu-id="c2d60-166">Other</span></span>

<span data-ttu-id="c2d60-167">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="c2d60-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="c2d60-168">значения свойств Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="c2d60-168">containerType property values</span></span>
<span data-ttu-id="c2d60-169">Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [оффицеграфинсигхтс](officegraphinsights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="c2d60-169">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="c2d60-170">Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".</span><span class="sxs-lookup"><span data-stu-id="c2d60-170">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="c2d60-171">онедривебусинесс</span><span class="sxs-lookup"><span data-stu-id="c2d60-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="c2d60-172">Site</span><span class="sxs-lookup"><span data-stu-id="c2d60-172">Site</span></span>
-   <span data-ttu-id="c2d60-173">Почта</span><span class="sxs-lookup"><span data-stu-id="c2d60-173">Mail</span></span>
-   <span data-ttu-id="c2d60-174">Оставляют</span><span class="sxs-lookup"><span data-stu-id="c2d60-174">DropBox</span></span>
-   <span data-ttu-id="c2d60-175">Box</span><span class="sxs-lookup"><span data-stu-id="c2d60-175">Box</span></span>
-   <span data-ttu-id="c2d60-176">гдриве</span><span class="sxs-lookup"><span data-stu-id="c2d60-176">GDrive</span></span>

<span data-ttu-id="c2d60-177">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="c2d60-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
