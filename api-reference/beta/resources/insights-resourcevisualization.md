---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a318ace2f69269a62cce728d1ececf01df97f3e0
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427391"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="69b65-103">Тип ресурса ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="69b65-103">resourceVisualization resource type</span></span>

<span data-ttu-id="69b65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69b65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69b65-105">Сложный тип, содержащий свойства [итеминсигхтс](iteminsights.md).</span><span class="sxs-lookup"><span data-stu-id="69b65-105">Complex type containing properties of [itemInsights](iteminsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="69b65-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69b65-106">JSON representation</span></span>

<span data-ttu-id="69b65-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="69b65-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="69b65-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="69b65-108">Properties</span></span>

| <span data-ttu-id="69b65-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="69b65-109">Property</span></span>              | <span data-ttu-id="69b65-110">Тип</span><span class="sxs-lookup"><span data-stu-id="69b65-110">Type</span></span>          | <span data-ttu-id="69b65-111">Описание</span><span class="sxs-lookup"><span data-stu-id="69b65-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="69b65-112">title</span><span class="sxs-lookup"><span data-stu-id="69b65-112">title</span></span>                 | <span data-ttu-id="69b65-113">String</span><span class="sxs-lookup"><span data-stu-id="69b65-113">String</span></span>        | <span data-ttu-id="69b65-114">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="69b65-114">The item's title text.</span></span>               |
| <span data-ttu-id="69b65-115">type</span><span class="sxs-lookup"><span data-stu-id="69b65-115">type</span></span>              | <span data-ttu-id="69b65-116">String</span><span class="sxs-lookup"><span data-stu-id="69b65-116">String</span></span>        | <span data-ttu-id="69b65-117">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="69b65-117">The item's media type.</span></span> <span data-ttu-id="69b65-118">Можно использовать для фильтрации определенного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="69b65-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="69b65-119">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="69b65-119">See below for supported types.</span></span> |
| <span data-ttu-id="69b65-120">MediaType</span><span class="sxs-lookup"><span data-stu-id="69b65-120">mediaType</span></span>             | <span data-ttu-id="69b65-121">String</span><span class="sxs-lookup"><span data-stu-id="69b65-121">String</span></span>        | <span data-ttu-id="69b65-122">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="69b65-122">The item's media type.</span></span> <span data-ttu-id="69b65-123">Может использоваться для фильтрации файлов определенного типа на основе поддерживаемых типов MIME MIME для устройства IANA.</span><span class="sxs-lookup"><span data-stu-id="69b65-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="69b65-124">Обратите внимание, что поддерживаются не все типы MIME мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="69b65-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="69b65-125">превиевимажеурл</span><span class="sxs-lookup"><span data-stu-id="69b65-125">previewImageUrl</span></span>       | <span data-ttu-id="69b65-126">String</span><span class="sxs-lookup"><span data-stu-id="69b65-126">String</span></span>        | <span data-ttu-id="69b65-127">URL-адрес, ведущая к изображению для предварительного просмотра элемента.</span><span class="sxs-lookup"><span data-stu-id="69b65-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="69b65-128">previewText</span><span class="sxs-lookup"><span data-stu-id="69b65-128">previewText</span></span>           | <span data-ttu-id="69b65-129">String</span><span class="sxs-lookup"><span data-stu-id="69b65-129">String</span></span>        | <span data-ttu-id="69b65-130">Предварительный текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="69b65-130">A preview text for the item.</span></span> |
| <span data-ttu-id="69b65-131">контаинервебурл</span><span class="sxs-lookup"><span data-stu-id="69b65-131">containerWebUrl</span></span>       | <span data-ttu-id="69b65-132">String</span><span class="sxs-lookup"><span data-stu-id="69b65-132">String</span></span>        | <span data-ttu-id="69b65-133">Путь, начинающийся с папки, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="69b65-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="69b65-134">контаинердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="69b65-134">containerDisplayName</span></span>  | <span data-ttu-id="69b65-135">String</span><span class="sxs-lookup"><span data-stu-id="69b65-135">String</span></span>        | <span data-ttu-id="69b65-136">Строка, описывающая место хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="69b65-136">A string describing where the item is stored.</span></span> <span data-ttu-id="69b65-137">Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="69b65-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="69b65-138">контаинертипе</span><span class="sxs-lookup"><span data-stu-id="69b65-138">containerType</span></span>         | <span data-ttu-id="69b65-139">String</span><span class="sxs-lookup"><span data-stu-id="69b65-139">String</span></span> | <span data-ttu-id="69b65-140">Можно использовать для фильтрации по типу контейнера, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="69b65-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="69b65-141">Например, site или Онедривебусинесс.</span><span class="sxs-lookup"><span data-stu-id="69b65-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="69b65-142">Ввод значений свойств</span><span class="sxs-lookup"><span data-stu-id="69b65-142">Type property values</span></span>
-   <span data-ttu-id="69b65-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="69b65-143">PowerPoint</span></span>
-   <span data-ttu-id="69b65-144">Word</span><span class="sxs-lookup"><span data-stu-id="69b65-144">Word</span></span>
-   <span data-ttu-id="69b65-145">Excel</span><span class="sxs-lookup"><span data-stu-id="69b65-145">Excel</span></span>
-   <span data-ttu-id="69b65-146">]</span><span class="sxs-lookup"><span data-stu-id="69b65-146">Pdf</span></span>
-   <span data-ttu-id="69b65-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="69b65-147">OneNote</span></span>
-   <span data-ttu-id="69b65-148">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="69b65-148">OneNotePage</span></span>
-   <span data-ttu-id="69b65-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="69b65-149">InfoPath</span></span>
-   <span data-ttu-id="69b65-150">Visio</span><span class="sxs-lookup"><span data-stu-id="69b65-150">Visio</span></span>
-   <span data-ttu-id="69b65-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="69b65-151">Publisher</span></span>
-   <span data-ttu-id="69b65-152">Project</span><span class="sxs-lookup"><span data-stu-id="69b65-152">Project</span></span>
-   <span data-ttu-id="69b65-153">Access</span><span class="sxs-lookup"><span data-stu-id="69b65-153">Access</span></span>
-   <span data-ttu-id="69b65-154">Почта</span><span class="sxs-lookup"><span data-stu-id="69b65-154">Mail</span></span>
-   <span data-ttu-id="69b65-155">Расширения</span><span class="sxs-lookup"><span data-stu-id="69b65-155">Csv</span></span>
-   <span data-ttu-id="69b65-156">Архив</span><span class="sxs-lookup"><span data-stu-id="69b65-156">Archive</span></span>
-   <span data-ttu-id="69b65-157">Компьютеров</span><span class="sxs-lookup"><span data-stu-id="69b65-157">Xps</span></span>
-   <span data-ttu-id="69b65-158">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="69b65-158">Audio</span></span>
-   <span data-ttu-id="69b65-159">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="69b65-159">Video</span></span>
-   <span data-ttu-id="69b65-160">Изображение</span><span class="sxs-lookup"><span data-stu-id="69b65-160">Image</span></span>
-   <span data-ttu-id="69b65-161">Web</span><span class="sxs-lookup"><span data-stu-id="69b65-161">Web</span></span>
-   <span data-ttu-id="69b65-162">Текст</span><span class="sxs-lookup"><span data-stu-id="69b65-162">Text</span></span>
-   <span data-ttu-id="69b65-163">Xml</span><span class="sxs-lookup"><span data-stu-id="69b65-163">Xml</span></span>
-   <span data-ttu-id="69b65-164">Story</span><span class="sxs-lookup"><span data-stu-id="69b65-164">Story</span></span>
-   <span data-ttu-id="69b65-165">екстерналконтент</span><span class="sxs-lookup"><span data-stu-id="69b65-165">ExternalContent</span></span>
-   <span data-ttu-id="69b65-166">Folder</span><span class="sxs-lookup"><span data-stu-id="69b65-166">Folder</span></span>
-   <span data-ttu-id="69b65-167">Другое</span><span class="sxs-lookup"><span data-stu-id="69b65-167">Other</span></span>

<span data-ttu-id="69b65-168">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="69b65-168">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="69b65-169">значения свойств Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="69b65-169">containerType property values</span></span>
<span data-ttu-id="69b65-170">Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [итеминсигхтс](iteminsights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="69b65-170">The supported types can differ based on containers from which [itemInsights](iteminsights.md) returns files.</span></span> <span data-ttu-id="69b65-171">Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".</span><span class="sxs-lookup"><span data-stu-id="69b65-171">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="69b65-172">онедривебусинесс</span><span class="sxs-lookup"><span data-stu-id="69b65-172">OneDriveBusiness</span></span>
-   <span data-ttu-id="69b65-173">Site</span><span class="sxs-lookup"><span data-stu-id="69b65-173">Site</span></span>
-   <span data-ttu-id="69b65-174">Почта</span><span class="sxs-lookup"><span data-stu-id="69b65-174">Mail</span></span>
-   <span data-ttu-id="69b65-175">Оставляют</span><span class="sxs-lookup"><span data-stu-id="69b65-175">DropBox</span></span>
-   <span data-ttu-id="69b65-176">Box</span><span class="sxs-lookup"><span data-stu-id="69b65-176">Box</span></span>
-   <span data-ttu-id="69b65-177">гдриве</span><span class="sxs-lookup"><span data-stu-id="69b65-177">GDrive</span></span>

<span data-ttu-id="69b65-178">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="69b65-178">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
