---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a8f6f048576ce5bc6ab532793d98fa1644e5158d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333570"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="e650d-103">Тип ресурса ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="e650d-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e650d-104">Сложный тип, содержащий свойства [аналитики](officegraphinsights.md).</span><span class="sxs-lookup"><span data-stu-id="e650d-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e650d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e650d-105">JSON representation</span></span>

<span data-ttu-id="e650d-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e650d-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e650d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e650d-107">Properties</span></span>

| <span data-ttu-id="e650d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e650d-108">Property</span></span>              | <span data-ttu-id="e650d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e650d-109">Type</span></span>          | <span data-ttu-id="e650d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e650d-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="e650d-111">title</span><span class="sxs-lookup"><span data-stu-id="e650d-111">title</span></span>                 | <span data-ttu-id="e650d-112">String</span><span class="sxs-lookup"><span data-stu-id="e650d-112">String</span></span>        | <span data-ttu-id="e650d-113">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="e650d-113">The item's title text.</span></span>               |
| <span data-ttu-id="e650d-114">type</span><span class="sxs-lookup"><span data-stu-id="e650d-114">type</span></span>              | <span data-ttu-id="e650d-115">String</span><span class="sxs-lookup"><span data-stu-id="e650d-115">String</span></span>        | <span data-ttu-id="e650d-116">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="e650d-116">The item's media type.</span></span> <span data-ttu-id="e650d-117">Можно использовать для фильтрации определенного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="e650d-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="e650d-118">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="e650d-118">See below for supported types.</span></span> |
| <span data-ttu-id="e650d-119">mediaType</span><span class="sxs-lookup"><span data-stu-id="e650d-119">mediaType</span></span>             | <span data-ttu-id="e650d-120">String</span><span class="sxs-lookup"><span data-stu-id="e650d-120">String</span></span>        | <span data-ttu-id="e650d-121">Тип мультимедиа элемента.</span><span class="sxs-lookup"><span data-stu-id="e650d-121">The item's media type.</span></span> <span data-ttu-id="e650d-122">Может использоваться для фильтрации для определенного типа файлов на основе поддерживаемых типов MIME для мультимедиа IANA.</span><span class="sxs-lookup"><span data-stu-id="e650d-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="e650d-123">Обратите внимание, что поддерживаются не все типы MIME мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="e650d-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="e650d-124">Превиевимажеурл</span><span class="sxs-lookup"><span data-stu-id="e650d-124">previewImageUrl</span></span>       | <span data-ttu-id="e650d-125">String</span><span class="sxs-lookup"><span data-stu-id="e650d-125">String</span></span>        | <span data-ttu-id="e650d-126">URL-адрес, ведущая к изображению для предварительного просмотра элемента.</span><span class="sxs-lookup"><span data-stu-id="e650d-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="e650d-127">previewText</span><span class="sxs-lookup"><span data-stu-id="e650d-127">previewText</span></span>           | <span data-ttu-id="e650d-128">String</span><span class="sxs-lookup"><span data-stu-id="e650d-128">String</span></span>        | <span data-ttu-id="e650d-129">Предварительный текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="e650d-129">A preview text for the item.</span></span> |
| <span data-ttu-id="e650d-130">Контаинервебурл</span><span class="sxs-lookup"><span data-stu-id="e650d-130">containerWebUrl</span></span>       | <span data-ttu-id="e650d-131">String</span><span class="sxs-lookup"><span data-stu-id="e650d-131">String</span></span>        | <span data-ttu-id="e650d-132">Путь, начинающийся с папки, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="e650d-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="e650d-133">Контаинердисплайнаме</span><span class="sxs-lookup"><span data-stu-id="e650d-133">containerDisplayName</span></span>  | <span data-ttu-id="e650d-134">String</span><span class="sxs-lookup"><span data-stu-id="e650d-134">String</span></span>        | <span data-ttu-id="e650d-135">Строка, описывающая место хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="e650d-135">A string describing where the item is stored.</span></span> <span data-ttu-id="e650d-136">Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="e650d-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="e650d-137">Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="e650d-137">containerType</span></span>         | <span data-ttu-id="e650d-138">String</span><span class="sxs-lookup"><span data-stu-id="e650d-138">String</span></span> | <span data-ttu-id="e650d-139">Можно использовать для фильтрации по типу контейнера, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="e650d-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="e650d-140">Например, site или Онедривебусинесс.</span><span class="sxs-lookup"><span data-stu-id="e650d-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="e650d-141">Ввод значений свойств</span><span class="sxs-lookup"><span data-stu-id="e650d-141">Type property values</span></span>
-   <span data-ttu-id="e650d-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="e650d-142">PowerPoint</span></span>
-   <span data-ttu-id="e650d-143">Word</span><span class="sxs-lookup"><span data-stu-id="e650d-143">Word</span></span>
-   <span data-ttu-id="e650d-144">Excel</span><span class="sxs-lookup"><span data-stu-id="e650d-144">Excel</span></span>
-   <span data-ttu-id="e650d-145">]</span><span class="sxs-lookup"><span data-stu-id="e650d-145">Pdf</span></span>
-   <span data-ttu-id="e650d-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="e650d-146">OneNote</span></span>
-   <span data-ttu-id="e650d-147">Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="e650d-147">OneNotePage</span></span>
-   <span data-ttu-id="e650d-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="e650d-148">InfoPath</span></span>
-   <span data-ttu-id="e650d-149">Visio</span><span class="sxs-lookup"><span data-stu-id="e650d-149">Visio</span></span>
-   <span data-ttu-id="e650d-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="e650d-150">Publisher</span></span>
-   <span data-ttu-id="e650d-151">Проект</span><span class="sxs-lookup"><span data-stu-id="e650d-151">Project</span></span>
-   <span data-ttu-id="e650d-152">Доступ</span><span class="sxs-lookup"><span data-stu-id="e650d-152">Access</span></span>
-   <span data-ttu-id="e650d-153">Почта</span><span class="sxs-lookup"><span data-stu-id="e650d-153">Mail</span></span>
-   <span data-ttu-id="e650d-154">Расширения</span><span class="sxs-lookup"><span data-stu-id="e650d-154">Csv</span></span>
-   <span data-ttu-id="e650d-155">Архив</span><span class="sxs-lookup"><span data-stu-id="e650d-155">Archive</span></span>
-   <span data-ttu-id="e650d-156">Компьютеров</span><span class="sxs-lookup"><span data-stu-id="e650d-156">Xps</span></span>
-   <span data-ttu-id="e650d-157">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="e650d-157">Audio</span></span>
-   <span data-ttu-id="e650d-158">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="e650d-158">Video</span></span>
-   <span data-ttu-id="e650d-159">Изображение</span><span class="sxs-lookup"><span data-stu-id="e650d-159">Image</span></span>
-   <span data-ttu-id="e650d-160">Веб</span><span class="sxs-lookup"><span data-stu-id="e650d-160">Web</span></span>
-   <span data-ttu-id="e650d-161">Текст</span><span class="sxs-lookup"><span data-stu-id="e650d-161">Text</span></span>
-   <span data-ttu-id="e650d-162">Xml</span><span class="sxs-lookup"><span data-stu-id="e650d-162">Xml</span></span>
-   <span data-ttu-id="e650d-163">Story</span><span class="sxs-lookup"><span data-stu-id="e650d-163">Story</span></span>
-   <span data-ttu-id="e650d-164">Екстерналконтент</span><span class="sxs-lookup"><span data-stu-id="e650d-164">ExternalContent</span></span>
-   <span data-ttu-id="e650d-165">Folder</span><span class="sxs-lookup"><span data-stu-id="e650d-165">Folder</span></span>
-   <span data-ttu-id="e650d-166">Прочее</span><span class="sxs-lookup"><span data-stu-id="e650d-166">Other</span></span>

<span data-ttu-id="e650d-167">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="e650d-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="e650d-168">значения свойств Контаинертипе</span><span class="sxs-lookup"><span data-stu-id="e650d-168">containerType property values</span></span>
<span data-ttu-id="e650d-169">Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [оффицеграфинсигхтс](officegraphinsights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="e650d-169">The supported types can differ based on containers from which [officeGraphInsights](officegraphinsights.md) returns files.</span></span> <span data-ttu-id="e650d-170">Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".</span><span class="sxs-lookup"><span data-stu-id="e650d-170">For example, only the [sharedInsight](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="e650d-171">Онедривебусинесс</span><span class="sxs-lookup"><span data-stu-id="e650d-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="e650d-172">site</span><span class="sxs-lookup"><span data-stu-id="e650d-172">Site</span></span>
-   <span data-ttu-id="e650d-173">Почта</span><span class="sxs-lookup"><span data-stu-id="e650d-173">Mail</span></span>
-   <span data-ttu-id="e650d-174">Оставляют</span><span class="sxs-lookup"><span data-stu-id="e650d-174">DropBox</span></span>
-   <span data-ttu-id="e650d-175">Box</span><span class="sxs-lookup"><span data-stu-id="e650d-175">Box</span></span>
-   <span data-ttu-id="e650d-176">Гдриве</span><span class="sxs-lookup"><span data-stu-id="e650d-176">GDrive</span></span>

<span data-ttu-id="e650d-177">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="e650d-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
