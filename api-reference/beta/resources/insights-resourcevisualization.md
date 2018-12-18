---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
author: simonhult
ms.openlocfilehash: d0c54895468fc9a01017e448df57c09c654616e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333539"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="b12b9-103">Тип ресурса resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="b12b9-103">resourceVisualization resource type</span></span>

> <span data-ttu-id="b12b9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b12b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b12b9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b12b9-106">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="b12b9-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b12b9-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b12b9-107">JSON representation</span></span>

<span data-ttu-id="b12b9-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="b12b9-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="b12b9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b12b9-109">Properties</span></span>

| <span data-ttu-id="b12b9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b12b9-110">Property</span></span>              | <span data-ttu-id="b12b9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b12b9-111">Type</span></span>          | <span data-ttu-id="b12b9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b12b9-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="b12b9-113">title</span><span class="sxs-lookup"><span data-stu-id="b12b9-113">title</span></span>                 | <span data-ttu-id="b12b9-114">Строка</span><span class="sxs-lookup"><span data-stu-id="b12b9-114">String</span></span>        | <span data-ttu-id="b12b9-115">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="b12b9-115">The item's title text.</span></span>               |
| <span data-ttu-id="b12b9-116">type</span><span class="sxs-lookup"><span data-stu-id="b12b9-116">type</span></span>              | <span data-ttu-id="b12b9-117">Строка</span><span class="sxs-lookup"><span data-stu-id="b12b9-117">String</span></span>        | <span data-ttu-id="b12b9-118">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b12b9-118">The item's media type.</span></span> <span data-ttu-id="b12b9-119">Можно использовать для фильтрации для конкретного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="b12b9-119">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="b12b9-120">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="b12b9-120">See below for supported types.</span></span> |
| <span data-ttu-id="b12b9-121">Тип носителя</span><span class="sxs-lookup"><span data-stu-id="b12b9-121">mediaType</span></span>             | <span data-ttu-id="b12b9-122">String.</span><span class="sxs-lookup"><span data-stu-id="b12b9-122">String</span></span>        | <span data-ttu-id="b12b9-123">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b12b9-123">The item's media type.</span></span> <span data-ttu-id="b12b9-124">Можно использовать для фильтрации для определенного типа файлов, поддерживаемые типы Mime IANA мультимедиа на основании.</span><span class="sxs-lookup"><span data-stu-id="b12b9-124">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="b12b9-125">Обратите внимание, что не все типы Mime мультимедиа поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b12b9-125">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="b12b9-126">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="b12b9-126">previewImageUrl</span></span>       | <span data-ttu-id="b12b9-127">String.</span><span class="sxs-lookup"><span data-stu-id="b12b9-127">String</span></span>        | <span data-ttu-id="b12b9-128">URL-адрес, приводя к изображения предварительного просмотра для элемента.</span><span class="sxs-lookup"><span data-stu-id="b12b9-128">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="b12b9-129">previewText</span><span class="sxs-lookup"><span data-stu-id="b12b9-129">previewText</span></span>           | <span data-ttu-id="b12b9-130">String.</span><span class="sxs-lookup"><span data-stu-id="b12b9-130">String</span></span>        | <span data-ttu-id="b12b9-131">Предварительная версия текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="b12b9-131">A preview text for the item.</span></span> |
| <span data-ttu-id="b12b9-132">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="b12b9-132">containerWebUrl</span></span>       | <span data-ttu-id="b12b9-133">String.</span><span class="sxs-lookup"><span data-stu-id="b12b9-133">String</span></span>        | <span data-ttu-id="b12b9-134">Путь, приводя к папке, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="b12b9-134">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="b12b9-135">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="b12b9-135">containerDisplayName</span></span>  | <span data-ttu-id="b12b9-136">String.</span><span class="sxs-lookup"><span data-stu-id="b12b9-136">String</span></span>        | <span data-ttu-id="b12b9-137">Строка, описывающая, где хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="b12b9-137">A string describing where the item is stored.</span></span> <span data-ttu-id="b12b9-138">Например имя сайт SharePoint или имя пользователя, определение владельца OneDrive, хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="b12b9-138">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="b12b9-139">containerType</span><span class="sxs-lookup"><span data-stu-id="b12b9-139">containerType</span></span>         | <span data-ttu-id="b12b9-140">String.</span><span class="sxs-lookup"><span data-stu-id="b12b9-140">String</span></span> | <span data-ttu-id="b12b9-141">Можно использовать для фильтрации по типу контейнер, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="b12b9-141">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="b12b9-142">Например, сайта или OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="b12b9-142">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="b12b9-143">Тип значения свойств</span><span class="sxs-lookup"><span data-stu-id="b12b9-143">Type property values</span></span>
-   <span data-ttu-id="b12b9-144">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="b12b9-144">PowerPoint</span></span>
-   <span data-ttu-id="b12b9-145">Word</span><span class="sxs-lookup"><span data-stu-id="b12b9-145">Word</span></span>
-   <span data-ttu-id="b12b9-146">Excel</span><span class="sxs-lookup"><span data-stu-id="b12b9-146">Excel</span></span>
-   <span data-ttu-id="b12b9-147">PDF</span><span class="sxs-lookup"><span data-stu-id="b12b9-147">Pdf</span></span>
-   <span data-ttu-id="b12b9-148">OneNote</span><span class="sxs-lookup"><span data-stu-id="b12b9-148">OneNote</span></span>
-   <span data-ttu-id="b12b9-149">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="b12b9-149">OneNotePage</span></span>
-   <span data-ttu-id="b12b9-150">InfoPath</span><span class="sxs-lookup"><span data-stu-id="b12b9-150">InfoPath</span></span>
-   <span data-ttu-id="b12b9-151">Visio</span><span class="sxs-lookup"><span data-stu-id="b12b9-151">Visio</span></span>
-   <span data-ttu-id="b12b9-152">Publisher</span><span class="sxs-lookup"><span data-stu-id="b12b9-152">Publisher</span></span>
-   <span data-ttu-id="b12b9-153">Project</span><span class="sxs-lookup"><span data-stu-id="b12b9-153">Project</span></span>
-   <span data-ttu-id="b12b9-154">Access</span><span class="sxs-lookup"><span data-stu-id="b12b9-154">Access</span></span>
-   <span data-ttu-id="b12b9-155">Почта</span><span class="sxs-lookup"><span data-stu-id="b12b9-155">Mail</span></span>
-   <span data-ttu-id="b12b9-156">CSV</span><span class="sxs-lookup"><span data-stu-id="b12b9-156">Csv</span></span>
-   <span data-ttu-id="b12b9-157">Archive</span><span class="sxs-lookup"><span data-stu-id="b12b9-157">Archive</span></span>
-   <span data-ttu-id="b12b9-158">XPS</span><span class="sxs-lookup"><span data-stu-id="b12b9-158">Xps</span></span>
-   <span data-ttu-id="b12b9-159">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="b12b9-159">Audio</span></span>
-   <span data-ttu-id="b12b9-160">Video (видео)</span><span class="sxs-lookup"><span data-stu-id="b12b9-160">Video</span></span>
-   <span data-ttu-id="b12b9-161">Изображение</span><span class="sxs-lookup"><span data-stu-id="b12b9-161">Image</span></span>
-   <span data-ttu-id="b12b9-162">Web</span><span class="sxs-lookup"><span data-stu-id="b12b9-162">Web</span></span>
-   <span data-ttu-id="b12b9-163">Текст</span><span class="sxs-lookup"><span data-stu-id="b12b9-163">Text</span></span>
-   <span data-ttu-id="b12b9-164">Xml</span><span class="sxs-lookup"><span data-stu-id="b12b9-164">Xml</span></span>
-   <span data-ttu-id="b12b9-165">Story</span><span class="sxs-lookup"><span data-stu-id="b12b9-165">Story</span></span>
-   <span data-ttu-id="b12b9-166">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="b12b9-166">ExternalContent</span></span>
-   <span data-ttu-id="b12b9-167">Folder</span><span class="sxs-lookup"><span data-stu-id="b12b9-167">Folder</span></span>
-   <span data-ttu-id="b12b9-168">Other</span><span class="sxs-lookup"><span data-stu-id="b12b9-168">Other</span></span>

<span data-ttu-id="b12b9-169">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="b12b9-169">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="b12b9-170">значения свойств containerType</span><span class="sxs-lookup"><span data-stu-id="b12b9-170">containerType property values</span></span>
<span data-ttu-id="b12b9-171">Поддерживаемые типы может отличаться в зависимости от контейнеров, с которых [возможность получения](insights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="b12b9-171">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="b12b9-172">Например только сведений об [общих](insights-shared.md) возвращает файлы из 'Общего банка данных», «Поле» и «GDrive».</span><span class="sxs-lookup"><span data-stu-id="b12b9-172">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="b12b9-173">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="b12b9-173">OneDriveBusiness</span></span>
-   <span data-ttu-id="b12b9-174">Site</span><span class="sxs-lookup"><span data-stu-id="b12b9-174">Site</span></span>
-   <span data-ttu-id="b12b9-175">Почта</span><span class="sxs-lookup"><span data-stu-id="b12b9-175">Mail</span></span>
-   <span data-ttu-id="b12b9-176">Общего банка данных</span><span class="sxs-lookup"><span data-stu-id="b12b9-176">DropBox</span></span>
-   <span data-ttu-id="b12b9-177">Box</span><span class="sxs-lookup"><span data-stu-id="b12b9-177">Box</span></span>
-   <span data-ttu-id="b12b9-178">GDrive</span><span class="sxs-lookup"><span data-stu-id="b12b9-178">GDrive</span></span>

<span data-ttu-id="b12b9-179">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="b12b9-179">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>