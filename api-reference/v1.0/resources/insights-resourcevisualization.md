---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 876acf56d4f3445d55163a8c4cdb5bc1461c45de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531294"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="e01fe-103">Тип ресурса ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="e01fe-103">resourceVisualization resource type</span></span>

<span data-ttu-id="e01fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e01fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e01fe-105">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="e01fe-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e01fe-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e01fe-106">JSON representation</span></span>

<span data-ttu-id="e01fe-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e01fe-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e01fe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e01fe-108">Properties</span></span>

| <span data-ttu-id="e01fe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e01fe-109">Property</span></span>              | <span data-ttu-id="e01fe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e01fe-110">Type</span></span>          | <span data-ttu-id="e01fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e01fe-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="e01fe-112">title</span><span class="sxs-lookup"><span data-stu-id="e01fe-112">title</span></span>                 | <span data-ttu-id="e01fe-113">String</span><span class="sxs-lookup"><span data-stu-id="e01fe-113">String</span></span>        | <span data-ttu-id="e01fe-114">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="e01fe-114">The item's title text.</span></span>               |
| <span data-ttu-id="e01fe-115">type</span><span class="sxs-lookup"><span data-stu-id="e01fe-115">type</span></span>              | <span data-ttu-id="e01fe-116">String</span><span class="sxs-lookup"><span data-stu-id="e01fe-116">String</span></span>        | <span data-ttu-id="e01fe-117">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="e01fe-117">The item's media type.</span></span> <span data-ttu-id="e01fe-118">Можно использовать для фильтрации определенного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="e01fe-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="e01fe-119">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="e01fe-119">See below for supported types.</span></span> |
| <span data-ttu-id="e01fe-120">mediaType</span><span class="sxs-lookup"><span data-stu-id="e01fe-120">mediaType</span></span>             | <span data-ttu-id="e01fe-121">String</span><span class="sxs-lookup"><span data-stu-id="e01fe-121">String</span></span>        | <span data-ttu-id="e01fe-122">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="e01fe-122">The item's media type.</span></span> <span data-ttu-id="e01fe-123">Может использоваться для фильтрации файлов определенного типа на основе поддерживаемых типов MIME MIME для устройства IANA.</span><span class="sxs-lookup"><span data-stu-id="e01fe-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="e01fe-124">Обратите внимание, что поддерживаются не все типы MIME мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e01fe-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="e01fe-125">превиевимажеурл</span><span class="sxs-lookup"><span data-stu-id="e01fe-125">previewImageUrl</span></span>       | <span data-ttu-id="e01fe-126">String</span><span class="sxs-lookup"><span data-stu-id="e01fe-126">String</span></span>        | <span data-ttu-id="e01fe-127">URL-адрес, ведущая к изображению для предварительного просмотра элемента.</span><span class="sxs-lookup"><span data-stu-id="e01fe-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="e01fe-128">previewText</span><span class="sxs-lookup"><span data-stu-id="e01fe-128">previewText</span></span>           | <span data-ttu-id="e01fe-129">String</span><span class="sxs-lookup"><span data-stu-id="e01fe-129">String</span></span>        | <span data-ttu-id="e01fe-130">Предварительный текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="e01fe-130">A preview text for the item.</span></span> |
| <span data-ttu-id="e01fe-131">контаинервебурл</span><span class="sxs-lookup"><span data-stu-id="e01fe-131">containerWebUrl</span></span>       | <span data-ttu-id="e01fe-132">String</span><span class="sxs-lookup"><span data-stu-id="e01fe-132">String</span></span>        | <span data-ttu-id="e01fe-133">Путь, начинающийся с папки, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="e01fe-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="e01fe-134">контаинердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="e01fe-134">containerDisplayName</span></span>  | <span data-ttu-id="e01fe-135">String</span><span class="sxs-lookup"><span data-stu-id="e01fe-135">String</span></span>        | <span data-ttu-id="e01fe-136">Строка, описывающая место хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="e01fe-136">A string describing where the item is stored.</span></span> <span data-ttu-id="e01fe-137">Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="e01fe-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="e01fe-138">контаинертипе</span><span class="sxs-lookup"><span data-stu-id="e01fe-138">containerType</span></span>         | <span data-ttu-id="e01fe-139">String</span><span class="sxs-lookup"><span data-stu-id="e01fe-139">String</span></span> | <span data-ttu-id="e01fe-140">Можно использовать для фильтрации по типу контейнера, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="e01fe-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="e01fe-141">Например, site или Онедривебусинесс.</span><span class="sxs-lookup"><span data-stu-id="e01fe-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="e01fe-142">Ввод значений свойств</span><span class="sxs-lookup"><span data-stu-id="e01fe-142">Type property values</span></span>
-   <span data-ttu-id="e01fe-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="e01fe-143">PowerPoint</span></span>
-   <span data-ttu-id="e01fe-144">Word</span><span class="sxs-lookup"><span data-stu-id="e01fe-144">Word</span></span>
-   <span data-ttu-id="e01fe-145">Excel</span><span class="sxs-lookup"><span data-stu-id="e01fe-145">Excel</span></span>
-   <span data-ttu-id="e01fe-146">]</span><span class="sxs-lookup"><span data-stu-id="e01fe-146">Pdf</span></span>
-   <span data-ttu-id="e01fe-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="e01fe-147">OneNote</span></span>
-   <span data-ttu-id="e01fe-148">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="e01fe-148">OneNotePage</span></span>
-   <span data-ttu-id="e01fe-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="e01fe-149">InfoPath</span></span>
-   <span data-ttu-id="e01fe-150">Visio</span><span class="sxs-lookup"><span data-stu-id="e01fe-150">Visio</span></span>
-   <span data-ttu-id="e01fe-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="e01fe-151">Publisher</span></span>
-   <span data-ttu-id="e01fe-152">Project</span><span class="sxs-lookup"><span data-stu-id="e01fe-152">Project</span></span>
-   <span data-ttu-id="e01fe-153">Access</span><span class="sxs-lookup"><span data-stu-id="e01fe-153">Access</span></span>
-   <span data-ttu-id="e01fe-154">Почта</span><span class="sxs-lookup"><span data-stu-id="e01fe-154">Mail</span></span>
-   <span data-ttu-id="e01fe-155">Расширения</span><span class="sxs-lookup"><span data-stu-id="e01fe-155">Csv</span></span>
-   <span data-ttu-id="e01fe-156">Архив</span><span class="sxs-lookup"><span data-stu-id="e01fe-156">Archive</span></span>
-   <span data-ttu-id="e01fe-157">Компьютеров</span><span class="sxs-lookup"><span data-stu-id="e01fe-157">Xps</span></span>
-   <span data-ttu-id="e01fe-158">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="e01fe-158">Audio</span></span>
-   <span data-ttu-id="e01fe-159">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="e01fe-159">Video</span></span>
-   <span data-ttu-id="e01fe-160">Изображение</span><span class="sxs-lookup"><span data-stu-id="e01fe-160">Image</span></span>
-   <span data-ttu-id="e01fe-161">Web</span><span class="sxs-lookup"><span data-stu-id="e01fe-161">Web</span></span>
-   <span data-ttu-id="e01fe-162">Текст</span><span class="sxs-lookup"><span data-stu-id="e01fe-162">Text</span></span>
-   <span data-ttu-id="e01fe-163">Xml</span><span class="sxs-lookup"><span data-stu-id="e01fe-163">Xml</span></span>
-   <span data-ttu-id="e01fe-164">Story</span><span class="sxs-lookup"><span data-stu-id="e01fe-164">Story</span></span>
-   <span data-ttu-id="e01fe-165">екстерналконтент</span><span class="sxs-lookup"><span data-stu-id="e01fe-165">ExternalContent</span></span>
-   <span data-ttu-id="e01fe-166">Folder</span><span class="sxs-lookup"><span data-stu-id="e01fe-166">Folder</span></span>
-   <span data-ttu-id="e01fe-167">Другое</span><span class="sxs-lookup"><span data-stu-id="e01fe-167">Other</span></span>

<span data-ttu-id="e01fe-168">Пример запроса:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="e01fe-168">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="e01fe-169">значения свойств Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="e01fe-169">containerType property values</span></span>
<span data-ttu-id="e01fe-170">Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [оффицеграфинсигхтс](officegraphinsights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="e01fe-170">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="e01fe-171">Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".</span><span class="sxs-lookup"><span data-stu-id="e01fe-171">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="e01fe-172">онедривебусинесс</span><span class="sxs-lookup"><span data-stu-id="e01fe-172">OneDriveBusiness</span></span>
-   <span data-ttu-id="e01fe-173">Site</span><span class="sxs-lookup"><span data-stu-id="e01fe-173">Site</span></span>
-   <span data-ttu-id="e01fe-174">Почта</span><span class="sxs-lookup"><span data-stu-id="e01fe-174">Mail</span></span>
-   <span data-ttu-id="e01fe-175">Оставляют</span><span class="sxs-lookup"><span data-stu-id="e01fe-175">DropBox</span></span>
-   <span data-ttu-id="e01fe-176">Box</span><span class="sxs-lookup"><span data-stu-id="e01fe-176">Box</span></span>
-   <span data-ttu-id="e01fe-177">гдриве</span><span class="sxs-lookup"><span data-stu-id="e01fe-177">GDrive</span></span>

<span data-ttu-id="e01fe-178">Пример запроса:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="e01fe-178">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
