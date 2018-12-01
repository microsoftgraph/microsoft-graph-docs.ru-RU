---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
ms.openlocfilehash: 3ed61a8547e072938fc073d90f2592baf4c08fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079873"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="d2dce-103">Тип ресурса resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="d2dce-103">resourceVisualization resource type</span></span>

> <span data-ttu-id="d2dce-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2dce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2dce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2dce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2dce-106">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="d2dce-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2dce-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2dce-107">JSON representation</span></span>

<span data-ttu-id="d2dce-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d2dce-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d2dce-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2dce-109">Properties</span></span>

| <span data-ttu-id="d2dce-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2dce-110">Property</span></span>              | <span data-ttu-id="d2dce-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d2dce-111">Type</span></span>          | <span data-ttu-id="d2dce-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d2dce-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="d2dce-113">title</span><span class="sxs-lookup"><span data-stu-id="d2dce-113">title</span></span>                 | <span data-ttu-id="d2dce-114">String</span><span class="sxs-lookup"><span data-stu-id="d2dce-114">String</span></span>        | <span data-ttu-id="d2dce-115">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="d2dce-115">The item's title text.</span></span>               |
| <span data-ttu-id="d2dce-116">type</span><span class="sxs-lookup"><span data-stu-id="d2dce-116">type</span></span>              | <span data-ttu-id="d2dce-117">String</span><span class="sxs-lookup"><span data-stu-id="d2dce-117">String</span></span>        | <span data-ttu-id="d2dce-118">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="d2dce-118">The item's media type.</span></span> <span data-ttu-id="d2dce-119">Можно использовать для фильтрации для конкретного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="d2dce-119">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="d2dce-120">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="d2dce-120">See below for supported types.</span></span> |
| <span data-ttu-id="d2dce-121">Тип носителя</span><span class="sxs-lookup"><span data-stu-id="d2dce-121">mediaType</span></span>             | <span data-ttu-id="d2dce-122">String</span><span class="sxs-lookup"><span data-stu-id="d2dce-122">String</span></span>        | <span data-ttu-id="d2dce-123">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="d2dce-123">The item's media type.</span></span> <span data-ttu-id="d2dce-124">Можно использовать для фильтрации для определенного типа файлов, поддерживаемые типы Mime IANA мультимедиа на основании.</span><span class="sxs-lookup"><span data-stu-id="d2dce-124">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="d2dce-125">Обратите внимание, что не все типы Mime мультимедиа поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="d2dce-125">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="d2dce-126">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="d2dce-126">previewImageUrl</span></span>       | <span data-ttu-id="d2dce-127">String</span><span class="sxs-lookup"><span data-stu-id="d2dce-127">String</span></span>        | <span data-ttu-id="d2dce-128">URL-адрес, приводя к изображения предварительного просмотра для элемента.</span><span class="sxs-lookup"><span data-stu-id="d2dce-128">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="d2dce-129">previewText</span><span class="sxs-lookup"><span data-stu-id="d2dce-129">previewText</span></span>           | <span data-ttu-id="d2dce-130">String</span><span class="sxs-lookup"><span data-stu-id="d2dce-130">String</span></span>        | <span data-ttu-id="d2dce-131">Предварительная версия текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="d2dce-131">A preview text for the item.</span></span> |
| <span data-ttu-id="d2dce-132">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="d2dce-132">containerWebUrl</span></span>       | <span data-ttu-id="d2dce-133">String</span><span class="sxs-lookup"><span data-stu-id="d2dce-133">String</span></span>        | <span data-ttu-id="d2dce-134">Путь, приводя к папке, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="d2dce-134">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="d2dce-135">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="d2dce-135">containerDisplayName</span></span>  | <span data-ttu-id="d2dce-136">String</span><span class="sxs-lookup"><span data-stu-id="d2dce-136">String</span></span>        | <span data-ttu-id="d2dce-137">Строка, описывающая, где хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="d2dce-137">A string describing where the item is stored.</span></span> <span data-ttu-id="d2dce-138">Например имя сайт SharePoint или имя пользователя, определение владельца OneDrive, хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="d2dce-138">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="d2dce-139">containerType</span><span class="sxs-lookup"><span data-stu-id="d2dce-139">containerType</span></span>         | <span data-ttu-id="d2dce-140">String</span><span class="sxs-lookup"><span data-stu-id="d2dce-140">String</span></span> | <span data-ttu-id="d2dce-141">Можно использовать для фильтрации по типу контейнер, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="d2dce-141">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="d2dce-142">Например, сайта или OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="d2dce-142">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="d2dce-143">Тип значения свойств</span><span class="sxs-lookup"><span data-stu-id="d2dce-143">Type property values</span></span>
-   <span data-ttu-id="d2dce-144">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="d2dce-144">PowerPoint</span></span>
-   <span data-ttu-id="d2dce-145">Word</span><span class="sxs-lookup"><span data-stu-id="d2dce-145">Word</span></span>
-   <span data-ttu-id="d2dce-146">Excel</span><span class="sxs-lookup"><span data-stu-id="d2dce-146">Excel</span></span>
-   <span data-ttu-id="d2dce-147">PDF</span><span class="sxs-lookup"><span data-stu-id="d2dce-147">Pdf</span></span>
-   <span data-ttu-id="d2dce-148">OneNote</span><span class="sxs-lookup"><span data-stu-id="d2dce-148">OneNote</span></span>
-   <span data-ttu-id="d2dce-149">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="d2dce-149">OneNotePage</span></span>
-   <span data-ttu-id="d2dce-150">InfoPath</span><span class="sxs-lookup"><span data-stu-id="d2dce-150">InfoPath</span></span>
-   <span data-ttu-id="d2dce-151">Visio</span><span class="sxs-lookup"><span data-stu-id="d2dce-151">Visio</span></span>
-   <span data-ttu-id="d2dce-152">Publisher</span><span class="sxs-lookup"><span data-stu-id="d2dce-152">Publisher</span></span>
-   <span data-ttu-id="d2dce-153">Project</span><span class="sxs-lookup"><span data-stu-id="d2dce-153">Project</span></span>
-   <span data-ttu-id="d2dce-154">Access</span><span class="sxs-lookup"><span data-stu-id="d2dce-154">Access</span></span>
-   <span data-ttu-id="d2dce-155">Почта</span><span class="sxs-lookup"><span data-stu-id="d2dce-155">Mail</span></span>
-   <span data-ttu-id="d2dce-156">CSV</span><span class="sxs-lookup"><span data-stu-id="d2dce-156">Csv</span></span>
-   <span data-ttu-id="d2dce-157">Archive</span><span class="sxs-lookup"><span data-stu-id="d2dce-157">Archive</span></span>
-   <span data-ttu-id="d2dce-158">XPS</span><span class="sxs-lookup"><span data-stu-id="d2dce-158">Xps</span></span>
-   <span data-ttu-id="d2dce-159">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="d2dce-159">Audio</span></span>
-   <span data-ttu-id="d2dce-160">Video (видео)</span><span class="sxs-lookup"><span data-stu-id="d2dce-160">Video</span></span>
-   <span data-ttu-id="d2dce-161">Изображение</span><span class="sxs-lookup"><span data-stu-id="d2dce-161">Image</span></span>
-   <span data-ttu-id="d2dce-162">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="d2dce-162">Web</span></span>
-   <span data-ttu-id="d2dce-163">Текст</span><span class="sxs-lookup"><span data-stu-id="d2dce-163">Text</span></span>
-   <span data-ttu-id="d2dce-164">Xml</span><span class="sxs-lookup"><span data-stu-id="d2dce-164">Xml</span></span>
-   <span data-ttu-id="d2dce-165">Story</span><span class="sxs-lookup"><span data-stu-id="d2dce-165">Story</span></span>
-   <span data-ttu-id="d2dce-166">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="d2dce-166">ExternalContent</span></span>
-   <span data-ttu-id="d2dce-167">Folder</span><span class="sxs-lookup"><span data-stu-id="d2dce-167">Folder</span></span>
-   <span data-ttu-id="d2dce-168">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="d2dce-168">Other</span></span>

<span data-ttu-id="d2dce-169">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="d2dce-169">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="d2dce-170">значения свойств containerType</span><span class="sxs-lookup"><span data-stu-id="d2dce-170">containerType property values</span></span>
<span data-ttu-id="d2dce-171">Поддерживаемые типы может отличаться в зависимости от контейнеров, с которых [возможность получения](insights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="d2dce-171">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="d2dce-172">Например только сведений об [общих](insights-shared.md) возвращает файлы из 'Общего банка данных», «Поле» и «GDrive».</span><span class="sxs-lookup"><span data-stu-id="d2dce-172">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="d2dce-173">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="d2dce-173">OneDriveBusiness</span></span>
-   <span data-ttu-id="d2dce-174">Сайт</span><span class="sxs-lookup"><span data-stu-id="d2dce-174">Site</span></span>
-   <span data-ttu-id="d2dce-175">Почта</span><span class="sxs-lookup"><span data-stu-id="d2dce-175">Mail</span></span>
-   <span data-ttu-id="d2dce-176">Общего банка данных</span><span class="sxs-lookup"><span data-stu-id="d2dce-176">DropBox</span></span>
-   <span data-ttu-id="d2dce-177">Box</span><span class="sxs-lookup"><span data-stu-id="d2dce-177">Box</span></span>
-   <span data-ttu-id="d2dce-178">GDrive</span><span class="sxs-lookup"><span data-stu-id="d2dce-178">GDrive</span></span>

<span data-ttu-id="d2dce-179">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="d2dce-179">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>