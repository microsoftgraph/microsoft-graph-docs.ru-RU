---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2480f55cf0e7ea12d9bfaf31941a943095f62c31
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898039"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="39c84-103">Тип ресурса ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="39c84-103">resourceVisualization resource type</span></span>

<span data-ttu-id="39c84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39c84-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39c84-105">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="39c84-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="39c84-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="39c84-106">JSON representation</span></span>

<span data-ttu-id="39c84-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="39c84-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="39c84-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="39c84-108">Properties</span></span>

| <span data-ttu-id="39c84-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="39c84-109">Property</span></span>              | <span data-ttu-id="39c84-110">Тип</span><span class="sxs-lookup"><span data-stu-id="39c84-110">Type</span></span>          | <span data-ttu-id="39c84-111">Описание</span><span class="sxs-lookup"><span data-stu-id="39c84-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="39c84-112">title</span><span class="sxs-lookup"><span data-stu-id="39c84-112">title</span></span>                 | <span data-ttu-id="39c84-113">String</span><span class="sxs-lookup"><span data-stu-id="39c84-113">String</span></span>        | <span data-ttu-id="39c84-114">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="39c84-114">The item's title text.</span></span>               |
| <span data-ttu-id="39c84-115">type</span><span class="sxs-lookup"><span data-stu-id="39c84-115">type</span></span>              | <span data-ttu-id="39c84-116">String</span><span class="sxs-lookup"><span data-stu-id="39c84-116">String</span></span>        | <span data-ttu-id="39c84-117">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="39c84-117">The item's media type.</span></span> <span data-ttu-id="39c84-118">Можно использовать для фильтрации определенного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="39c84-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="39c84-119">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="39c84-119">See below for supported types.</span></span> |
| <span data-ttu-id="39c84-120">mediaType</span><span class="sxs-lookup"><span data-stu-id="39c84-120">mediaType</span></span>             | <span data-ttu-id="39c84-121">String</span><span class="sxs-lookup"><span data-stu-id="39c84-121">String</span></span>        | <span data-ttu-id="39c84-122">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="39c84-122">The item's media type.</span></span> <span data-ttu-id="39c84-123">Может использоваться для фильтрации файлов определенного типа на основе поддерживаемых типов MIME MIME для устройства IANA.</span><span class="sxs-lookup"><span data-stu-id="39c84-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="39c84-124">Обратите внимание, что поддерживаются не все типы MIME мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="39c84-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="39c84-125">превиевимажеурл</span><span class="sxs-lookup"><span data-stu-id="39c84-125">previewImageUrl</span></span>       | <span data-ttu-id="39c84-126">String</span><span class="sxs-lookup"><span data-stu-id="39c84-126">String</span></span>        | <span data-ttu-id="39c84-127">URL-адрес, ведущая к изображению для предварительного просмотра элемента.</span><span class="sxs-lookup"><span data-stu-id="39c84-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="39c84-128">previewText</span><span class="sxs-lookup"><span data-stu-id="39c84-128">previewText</span></span>           | <span data-ttu-id="39c84-129">String</span><span class="sxs-lookup"><span data-stu-id="39c84-129">String</span></span>        | <span data-ttu-id="39c84-130">Предварительный текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="39c84-130">A preview text for the item.</span></span> |
| <span data-ttu-id="39c84-131">контаинервебурл</span><span class="sxs-lookup"><span data-stu-id="39c84-131">containerWebUrl</span></span>       | <span data-ttu-id="39c84-132">String</span><span class="sxs-lookup"><span data-stu-id="39c84-132">String</span></span>        | <span data-ttu-id="39c84-133">Путь, начинающийся с папки, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="39c84-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="39c84-134">контаинердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="39c84-134">containerDisplayName</span></span>  | <span data-ttu-id="39c84-135">String</span><span class="sxs-lookup"><span data-stu-id="39c84-135">String</span></span>        | <span data-ttu-id="39c84-136">Строка, описывающая место хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="39c84-136">A string describing where the item is stored.</span></span> <span data-ttu-id="39c84-137">Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="39c84-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="39c84-138">контаинертипе</span><span class="sxs-lookup"><span data-stu-id="39c84-138">containerType</span></span>         | <span data-ttu-id="39c84-139">String</span><span class="sxs-lookup"><span data-stu-id="39c84-139">String</span></span> | <span data-ttu-id="39c84-140">Можно использовать для фильтрации по типу контейнера, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="39c84-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="39c84-141">Например, site или Онедривебусинесс.</span><span class="sxs-lookup"><span data-stu-id="39c84-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="39c84-142">Ввод значений свойств</span><span class="sxs-lookup"><span data-stu-id="39c84-142">Type property values</span></span>
-   <span data-ttu-id="39c84-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="39c84-143">PowerPoint</span></span>
-   <span data-ttu-id="39c84-144">Word</span><span class="sxs-lookup"><span data-stu-id="39c84-144">Word</span></span>
-   <span data-ttu-id="39c84-145">Excel</span><span class="sxs-lookup"><span data-stu-id="39c84-145">Excel</span></span>
-   <span data-ttu-id="39c84-146">]</span><span class="sxs-lookup"><span data-stu-id="39c84-146">Pdf</span></span>
-   <span data-ttu-id="39c84-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="39c84-147">OneNote</span></span>
-   <span data-ttu-id="39c84-148">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="39c84-148">OneNotePage</span></span>
-   <span data-ttu-id="39c84-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="39c84-149">InfoPath</span></span>
-   <span data-ttu-id="39c84-150">Visio</span><span class="sxs-lookup"><span data-stu-id="39c84-150">Visio</span></span>
-   <span data-ttu-id="39c84-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="39c84-151">Publisher</span></span>
-   <span data-ttu-id="39c84-152">Project</span><span class="sxs-lookup"><span data-stu-id="39c84-152">Project</span></span>
-   <span data-ttu-id="39c84-153">Доступ</span><span class="sxs-lookup"><span data-stu-id="39c84-153">Access</span></span>
-   <span data-ttu-id="39c84-154">Почта</span><span class="sxs-lookup"><span data-stu-id="39c84-154">Mail</span></span>
-   <span data-ttu-id="39c84-155">Расширения</span><span class="sxs-lookup"><span data-stu-id="39c84-155">Csv</span></span>
-   <span data-ttu-id="39c84-156">Архив</span><span class="sxs-lookup"><span data-stu-id="39c84-156">Archive</span></span>
-   <span data-ttu-id="39c84-157">Компьютеров</span><span class="sxs-lookup"><span data-stu-id="39c84-157">Xps</span></span>
-   <span data-ttu-id="39c84-158">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="39c84-158">Audio</span></span>
-   <span data-ttu-id="39c84-159">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="39c84-159">Video</span></span>
-   <span data-ttu-id="39c84-160">Изображение</span><span class="sxs-lookup"><span data-stu-id="39c84-160">Image</span></span>
-   <span data-ttu-id="39c84-161">Web</span><span class="sxs-lookup"><span data-stu-id="39c84-161">Web</span></span>
-   <span data-ttu-id="39c84-162">Текст</span><span class="sxs-lookup"><span data-stu-id="39c84-162">Text</span></span>
-   <span data-ttu-id="39c84-163">Xml</span><span class="sxs-lookup"><span data-stu-id="39c84-163">Xml</span></span>
-   <span data-ttu-id="39c84-164">Story</span><span class="sxs-lookup"><span data-stu-id="39c84-164">Story</span></span>
-   <span data-ttu-id="39c84-165">екстерналконтент</span><span class="sxs-lookup"><span data-stu-id="39c84-165">ExternalContent</span></span>
-   <span data-ttu-id="39c84-166">Folder</span><span class="sxs-lookup"><span data-stu-id="39c84-166">Folder</span></span>
- <span data-ttu-id="39c84-167">SPSite</span><span class="sxs-lookup"><span data-stu-id="39c84-167">Spsite</span></span>
-   <span data-ttu-id="39c84-168">Другое</span><span class="sxs-lookup"><span data-stu-id="39c84-168">Other</span></span>

<span data-ttu-id="39c84-169">Пример запроса:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="39c84-169">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

<span data-ttu-id="39c84-170">Примечания: для `spsite` получения допустимых результатов может потребоваться выполнить сортировку по `lastUsed/lastAccessedDateTime` возрастанию.</span><span class="sxs-lookup"><span data-stu-id="39c84-170">Notes: For `spsite` you may need to sort by `lastUsed/lastAccessedDateTime` desc in order to retrieve valid results</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="39c84-171">значения свойств Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="39c84-171">containerType property values</span></span>
<span data-ttu-id="39c84-172">Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [оффицеграфинсигхтс](officegraphinsights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="39c84-172">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="39c84-173">Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".</span><span class="sxs-lookup"><span data-stu-id="39c84-173">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="39c84-174">онедривебусинесс</span><span class="sxs-lookup"><span data-stu-id="39c84-174">OneDriveBusiness</span></span>
-   <span data-ttu-id="39c84-175">Site</span><span class="sxs-lookup"><span data-stu-id="39c84-175">Site</span></span>
-   <span data-ttu-id="39c84-176">Почта</span><span class="sxs-lookup"><span data-stu-id="39c84-176">Mail</span></span>
-   <span data-ttu-id="39c84-177">Оставляют</span><span class="sxs-lookup"><span data-stu-id="39c84-177">DropBox</span></span>
-   <span data-ttu-id="39c84-178">Box</span><span class="sxs-lookup"><span data-stu-id="39c84-178">Box</span></span>
-   <span data-ttu-id="39c84-179">гдриве</span><span class="sxs-lookup"><span data-stu-id="39c84-179">GDrive</span></span>

<span data-ttu-id="39c84-180">Пример запроса:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="39c84-180">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
