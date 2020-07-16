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
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="1d034-103">Тип ресурса ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="1d034-103">resourceVisualization resource type</span></span>

<span data-ttu-id="1d034-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d034-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d034-105">Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="1d034-105">Complex type containing properties of [officeGraphInsights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d034-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1d034-106">JSON representation</span></span>

<span data-ttu-id="1d034-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="1d034-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="1d034-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d034-108">Properties</span></span>

| <span data-ttu-id="1d034-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d034-109">Property</span></span>              | <span data-ttu-id="1d034-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1d034-110">Type</span></span>          | <span data-ttu-id="1d034-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1d034-111">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="1d034-112">title</span><span class="sxs-lookup"><span data-stu-id="1d034-112">title</span></span>                 | <span data-ttu-id="1d034-113">String</span><span class="sxs-lookup"><span data-stu-id="1d034-113">String</span></span>        | <span data-ttu-id="1d034-114">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="1d034-114">The item's title text.</span></span>               |
| <span data-ttu-id="1d034-115">type</span><span class="sxs-lookup"><span data-stu-id="1d034-115">type</span></span>              | <span data-ttu-id="1d034-116">String</span><span class="sxs-lookup"><span data-stu-id="1d034-116">String</span></span>        | <span data-ttu-id="1d034-117">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="1d034-117">The item's media type.</span></span> <span data-ttu-id="1d034-118">Можно использовать для фильтрации определенного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="1d034-118">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="1d034-119">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="1d034-119">See below for supported types.</span></span> |
| <span data-ttu-id="1d034-120">mediaType</span><span class="sxs-lookup"><span data-stu-id="1d034-120">mediaType</span></span>             | <span data-ttu-id="1d034-121">String</span><span class="sxs-lookup"><span data-stu-id="1d034-121">String</span></span>        | <span data-ttu-id="1d034-122">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="1d034-122">The item's media type.</span></span> <span data-ttu-id="1d034-123">Может использоваться для фильтрации файлов определенного типа на основе поддерживаемых типов MIME MIME для устройства IANA.</span><span class="sxs-lookup"><span data-stu-id="1d034-123">Can be used for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="1d034-124">Обратите внимание, что поддерживаются не все типы MIME мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="1d034-124">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="1d034-125">превиевимажеурл</span><span class="sxs-lookup"><span data-stu-id="1d034-125">previewImageUrl</span></span>       | <span data-ttu-id="1d034-126">String</span><span class="sxs-lookup"><span data-stu-id="1d034-126">String</span></span>        | <span data-ttu-id="1d034-127">URL-адрес, ведущая к изображению для предварительного просмотра элемента.</span><span class="sxs-lookup"><span data-stu-id="1d034-127">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="1d034-128">previewText</span><span class="sxs-lookup"><span data-stu-id="1d034-128">previewText</span></span>           | <span data-ttu-id="1d034-129">String</span><span class="sxs-lookup"><span data-stu-id="1d034-129">String</span></span>        | <span data-ttu-id="1d034-130">Предварительный текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="1d034-130">A preview text for the item.</span></span> |
| <span data-ttu-id="1d034-131">контаинервебурл</span><span class="sxs-lookup"><span data-stu-id="1d034-131">containerWebUrl</span></span>       | <span data-ttu-id="1d034-132">String</span><span class="sxs-lookup"><span data-stu-id="1d034-132">String</span></span>        | <span data-ttu-id="1d034-133">Путь, начинающийся с папки, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="1d034-133">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="1d034-134">контаинердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="1d034-134">containerDisplayName</span></span>  | <span data-ttu-id="1d034-135">String</span><span class="sxs-lookup"><span data-stu-id="1d034-135">String</span></span>        | <span data-ttu-id="1d034-136">Строка, описывающая место хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="1d034-136">A string describing where the item is stored.</span></span> <span data-ttu-id="1d034-137">Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="1d034-137">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="1d034-138">контаинертипе</span><span class="sxs-lookup"><span data-stu-id="1d034-138">containerType</span></span>         | <span data-ttu-id="1d034-139">String</span><span class="sxs-lookup"><span data-stu-id="1d034-139">String</span></span> | <span data-ttu-id="1d034-140">Можно использовать для фильтрации по типу контейнера, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="1d034-140">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="1d034-141">Например, site или Онедривебусинесс.</span><span class="sxs-lookup"><span data-stu-id="1d034-141">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="1d034-142">Ввод значений свойств</span><span class="sxs-lookup"><span data-stu-id="1d034-142">Type property values</span></span>
-   <span data-ttu-id="1d034-143">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="1d034-143">PowerPoint</span></span>
-   <span data-ttu-id="1d034-144">Word</span><span class="sxs-lookup"><span data-stu-id="1d034-144">Word</span></span>
-   <span data-ttu-id="1d034-145">Excel</span><span class="sxs-lookup"><span data-stu-id="1d034-145">Excel</span></span>
-   <span data-ttu-id="1d034-146">]</span><span class="sxs-lookup"><span data-stu-id="1d034-146">Pdf</span></span>
-   <span data-ttu-id="1d034-147">OneNote</span><span class="sxs-lookup"><span data-stu-id="1d034-147">OneNote</span></span>
-   <span data-ttu-id="1d034-148">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="1d034-148">OneNotePage</span></span>
-   <span data-ttu-id="1d034-149">InfoPath</span><span class="sxs-lookup"><span data-stu-id="1d034-149">InfoPath</span></span>
-   <span data-ttu-id="1d034-150">Visio</span><span class="sxs-lookup"><span data-stu-id="1d034-150">Visio</span></span>
-   <span data-ttu-id="1d034-151">Publisher</span><span class="sxs-lookup"><span data-stu-id="1d034-151">Publisher</span></span>
-   <span data-ttu-id="1d034-152">Project</span><span class="sxs-lookup"><span data-stu-id="1d034-152">Project</span></span>
-   <span data-ttu-id="1d034-153">Доступ</span><span class="sxs-lookup"><span data-stu-id="1d034-153">Access</span></span>
-   <span data-ttu-id="1d034-154">Почта</span><span class="sxs-lookup"><span data-stu-id="1d034-154">Mail</span></span>
-   <span data-ttu-id="1d034-155">Расширения</span><span class="sxs-lookup"><span data-stu-id="1d034-155">Csv</span></span>
-   <span data-ttu-id="1d034-156">Архив</span><span class="sxs-lookup"><span data-stu-id="1d034-156">Archive</span></span>
-   <span data-ttu-id="1d034-157">Компьютеров</span><span class="sxs-lookup"><span data-stu-id="1d034-157">Xps</span></span>
-   <span data-ttu-id="1d034-158">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="1d034-158">Audio</span></span>
-   <span data-ttu-id="1d034-159">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="1d034-159">Video</span></span>
-   <span data-ttu-id="1d034-160">Изображение</span><span class="sxs-lookup"><span data-stu-id="1d034-160">Image</span></span>
-   <span data-ttu-id="1d034-161">Web</span><span class="sxs-lookup"><span data-stu-id="1d034-161">Web</span></span>
-   <span data-ttu-id="1d034-162">Текст</span><span class="sxs-lookup"><span data-stu-id="1d034-162">Text</span></span>
-   <span data-ttu-id="1d034-163">Xml</span><span class="sxs-lookup"><span data-stu-id="1d034-163">Xml</span></span>
-   <span data-ttu-id="1d034-164">Story</span><span class="sxs-lookup"><span data-stu-id="1d034-164">Story</span></span>
-   <span data-ttu-id="1d034-165">екстерналконтент</span><span class="sxs-lookup"><span data-stu-id="1d034-165">ExternalContent</span></span>
-   <span data-ttu-id="1d034-166">Folder</span><span class="sxs-lookup"><span data-stu-id="1d034-166">Folder</span></span>
- <span data-ttu-id="1d034-167">SPSite</span><span class="sxs-lookup"><span data-stu-id="1d034-167">Spsite</span></span>
-   <span data-ttu-id="1d034-168">Другое</span><span class="sxs-lookup"><span data-stu-id="1d034-168">Other</span></span>

<span data-ttu-id="1d034-169">Пример запроса:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="1d034-169">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

<span data-ttu-id="1d034-170">Примечания: для `spsite` получения допустимых результатов может потребоваться выполнить сортировку по `lastUsed/lastAccessedDateTime` возрастанию.</span><span class="sxs-lookup"><span data-stu-id="1d034-170">Notes: For `spsite` you may need to sort by `lastUsed/lastAccessedDateTime` desc in order to retrieve valid results</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="1d034-171">значения свойств Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="1d034-171">containerType property values</span></span>
<span data-ttu-id="1d034-172">Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [оффицеграфинсигхтс](officegraphinsights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="1d034-172">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="1d034-173">Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".</span><span class="sxs-lookup"><span data-stu-id="1d034-173">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="1d034-174">онедривебусинесс</span><span class="sxs-lookup"><span data-stu-id="1d034-174">OneDriveBusiness</span></span>
-   <span data-ttu-id="1d034-175">Site</span><span class="sxs-lookup"><span data-stu-id="1d034-175">Site</span></span>
-   <span data-ttu-id="1d034-176">Почта</span><span class="sxs-lookup"><span data-stu-id="1d034-176">Mail</span></span>
-   <span data-ttu-id="1d034-177">Оставляют</span><span class="sxs-lookup"><span data-stu-id="1d034-177">DropBox</span></span>
-   <span data-ttu-id="1d034-178">Box</span><span class="sxs-lookup"><span data-stu-id="1d034-178">Box</span></span>
-   <span data-ttu-id="1d034-179">гдриве</span><span class="sxs-lookup"><span data-stu-id="1d034-179">GDrive</span></span>

<span data-ttu-id="1d034-180">Пример запроса:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="1d034-180">Example query: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
