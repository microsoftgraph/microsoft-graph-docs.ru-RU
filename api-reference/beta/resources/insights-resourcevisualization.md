---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 7600c843e36e3bce6c8a4182e0bfda14ad21d7b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844978"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="04814-103">Тип ресурса resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="04814-103">resourceVisualization resource type</span></span>

> <span data-ttu-id="04814-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04814-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04814-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04814-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04814-106">Сложный тип, содержащий свойства [средствами](insights.md).</span><span class="sxs-lookup"><span data-stu-id="04814-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="04814-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04814-107">JSON representation</span></span>

<span data-ttu-id="04814-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="04814-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="04814-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="04814-109">Properties</span></span>

| <span data-ttu-id="04814-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="04814-110">Property</span></span>              | <span data-ttu-id="04814-111">Тип</span><span class="sxs-lookup"><span data-stu-id="04814-111">Type</span></span>          | <span data-ttu-id="04814-112">Описание</span><span class="sxs-lookup"><span data-stu-id="04814-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="04814-113">title</span><span class="sxs-lookup"><span data-stu-id="04814-113">title</span></span>                 | <span data-ttu-id="04814-114">Строка</span><span class="sxs-lookup"><span data-stu-id="04814-114">String</span></span>        | <span data-ttu-id="04814-115">Текст заголовка элемента.</span><span class="sxs-lookup"><span data-stu-id="04814-115">The item's title text.</span></span>               |
| <span data-ttu-id="04814-116">type</span><span class="sxs-lookup"><span data-stu-id="04814-116">type</span></span>              | <span data-ttu-id="04814-117">Строка</span><span class="sxs-lookup"><span data-stu-id="04814-117">String</span></span>        | <span data-ttu-id="04814-118">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="04814-118">The item's media type.</span></span> <span data-ttu-id="04814-119">Можно использовать для фильтрации для конкретного файла на основе определенного типа.</span><span class="sxs-lookup"><span data-stu-id="04814-119">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="04814-120">Ниже приведены поддерживаемые типы.</span><span class="sxs-lookup"><span data-stu-id="04814-120">See below for supported types.</span></span> |
| <span data-ttu-id="04814-121">Тип носителя</span><span class="sxs-lookup"><span data-stu-id="04814-121">mediaType</span></span>             | <span data-ttu-id="04814-122">Строка</span><span class="sxs-lookup"><span data-stu-id="04814-122">String</span></span>        | <span data-ttu-id="04814-123">Тип элемента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="04814-123">The item's media type.</span></span> <span data-ttu-id="04814-124">Можно использовать для фильтрации для определенного типа файлов, поддерживаемые типы Mime IANA мультимедиа на основании.</span><span class="sxs-lookup"><span data-stu-id="04814-124">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="04814-125">Обратите внимание, что не все типы Mime мультимедиа поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="04814-125">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="04814-126">previewImageUrl</span><span class="sxs-lookup"><span data-stu-id="04814-126">previewImageUrl</span></span>       | <span data-ttu-id="04814-127">Строка</span><span class="sxs-lookup"><span data-stu-id="04814-127">String</span></span>        | <span data-ttu-id="04814-128">URL-адрес, приводя к изображения предварительного просмотра для элемента.</span><span class="sxs-lookup"><span data-stu-id="04814-128">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="04814-129">previewText</span><span class="sxs-lookup"><span data-stu-id="04814-129">previewText</span></span>           | <span data-ttu-id="04814-130">Строка</span><span class="sxs-lookup"><span data-stu-id="04814-130">String</span></span>        | <span data-ttu-id="04814-131">Предварительная версия текст для элемента.</span><span class="sxs-lookup"><span data-stu-id="04814-131">A preview text for the item.</span></span> |
| <span data-ttu-id="04814-132">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="04814-132">containerWebUrl</span></span>       | <span data-ttu-id="04814-133">Строка</span><span class="sxs-lookup"><span data-stu-id="04814-133">String</span></span>        | <span data-ttu-id="04814-134">Путь, приводя к папке, в которой хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="04814-134">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="04814-135">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="04814-135">containerDisplayName</span></span>  | <span data-ttu-id="04814-136">Строка</span><span class="sxs-lookup"><span data-stu-id="04814-136">String</span></span>        | <span data-ttu-id="04814-137">Строка, описывающая, где хранится элемент.</span><span class="sxs-lookup"><span data-stu-id="04814-137">A string describing where the item is stored.</span></span> <span data-ttu-id="04814-138">Например имя сайт SharePoint или имя пользователя, определение владельца OneDrive, хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="04814-138">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="04814-139">containerType</span><span class="sxs-lookup"><span data-stu-id="04814-139">containerType</span></span>         | <span data-ttu-id="04814-140">Строка</span><span class="sxs-lookup"><span data-stu-id="04814-140">String</span></span> | <span data-ttu-id="04814-141">Можно использовать для фильтрации по типу контейнер, в котором хранится файл.</span><span class="sxs-lookup"><span data-stu-id="04814-141">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="04814-142">Например, сайта или OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="04814-142">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="04814-143">Тип значения свойств</span><span class="sxs-lookup"><span data-stu-id="04814-143">Type property values</span></span>
-   <span data-ttu-id="04814-144">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="04814-144">PowerPoint</span></span>
-   <span data-ttu-id="04814-145">Word</span><span class="sxs-lookup"><span data-stu-id="04814-145">Word</span></span>
-   <span data-ttu-id="04814-146">Excel</span><span class="sxs-lookup"><span data-stu-id="04814-146">Excel</span></span>
-   <span data-ttu-id="04814-147">PDF</span><span class="sxs-lookup"><span data-stu-id="04814-147">Pdf</span></span>
-   <span data-ttu-id="04814-148">OneNote</span><span class="sxs-lookup"><span data-stu-id="04814-148">OneNote</span></span>
-   <span data-ttu-id="04814-149">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="04814-149">OneNotePage</span></span>
-   <span data-ttu-id="04814-150">InfoPath</span><span class="sxs-lookup"><span data-stu-id="04814-150">InfoPath</span></span>
-   <span data-ttu-id="04814-151">Visio</span><span class="sxs-lookup"><span data-stu-id="04814-151">Visio</span></span>
-   <span data-ttu-id="04814-152">Publisher</span><span class="sxs-lookup"><span data-stu-id="04814-152">Publisher</span></span>
-   <span data-ttu-id="04814-153">Project</span><span class="sxs-lookup"><span data-stu-id="04814-153">Project</span></span>
-   <span data-ttu-id="04814-154">Access</span><span class="sxs-lookup"><span data-stu-id="04814-154">Access</span></span>
-   <span data-ttu-id="04814-155">Почта</span><span class="sxs-lookup"><span data-stu-id="04814-155">Mail</span></span>
-   <span data-ttu-id="04814-156">CSV</span><span class="sxs-lookup"><span data-stu-id="04814-156">Csv</span></span>
-   <span data-ttu-id="04814-157">Archive</span><span class="sxs-lookup"><span data-stu-id="04814-157">Archive</span></span>
-   <span data-ttu-id="04814-158">XPS</span><span class="sxs-lookup"><span data-stu-id="04814-158">Xps</span></span>
-   <span data-ttu-id="04814-159">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="04814-159">Audio</span></span>
-   <span data-ttu-id="04814-160">Video (видео)</span><span class="sxs-lookup"><span data-stu-id="04814-160">Video</span></span>
-   <span data-ttu-id="04814-161">Изображение</span><span class="sxs-lookup"><span data-stu-id="04814-161">Image</span></span>
-   <span data-ttu-id="04814-162">Веб</span><span class="sxs-lookup"><span data-stu-id="04814-162">Web</span></span>
-   <span data-ttu-id="04814-163">Текст</span><span class="sxs-lookup"><span data-stu-id="04814-163">Text</span></span>
-   <span data-ttu-id="04814-164">Xml</span><span class="sxs-lookup"><span data-stu-id="04814-164">Xml</span></span>
-   <span data-ttu-id="04814-165">Story</span><span class="sxs-lookup"><span data-stu-id="04814-165">Story</span></span>
-   <span data-ttu-id="04814-166">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="04814-166">ExternalContent</span></span>
-   <span data-ttu-id="04814-167">Folder</span><span class="sxs-lookup"><span data-stu-id="04814-167">Folder</span></span>
-   <span data-ttu-id="04814-168">Другое</span><span class="sxs-lookup"><span data-stu-id="04814-168">Other</span></span>

<span data-ttu-id="04814-169">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="04814-169">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="04814-170">значения свойств containerType</span><span class="sxs-lookup"><span data-stu-id="04814-170">containerType property values</span></span>
<span data-ttu-id="04814-171">Поддерживаемые типы может отличаться в зависимости от контейнеров, с которых [возможность получения](insights.md) возвращает файлы.</span><span class="sxs-lookup"><span data-stu-id="04814-171">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="04814-172">Например только сведений об [общих](insights-shared.md) возвращает файлы из 'Общего банка данных», «Поле» и «GDrive».</span><span class="sxs-lookup"><span data-stu-id="04814-172">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="04814-173">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="04814-173">OneDriveBusiness</span></span>
-   <span data-ttu-id="04814-174">Site</span><span class="sxs-lookup"><span data-stu-id="04814-174">Site</span></span>
-   <span data-ttu-id="04814-175">Почта</span><span class="sxs-lookup"><span data-stu-id="04814-175">Mail</span></span>
-   <span data-ttu-id="04814-176">Общего банка данных</span><span class="sxs-lookup"><span data-stu-id="04814-176">DropBox</span></span>
-   <span data-ttu-id="04814-177">Box</span><span class="sxs-lookup"><span data-stu-id="04814-177">Box</span></span>
-   <span data-ttu-id="04814-178">GDrive</span><span class="sxs-lookup"><span data-stu-id="04814-178">GDrive</span></span>

<span data-ttu-id="04814-179">Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="04814-179">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
