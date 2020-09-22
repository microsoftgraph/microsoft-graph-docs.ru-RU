---
title: Тип ресурса Арчиведпринтжоб
description: Запись "конечного состояния" (выполненного, прерванного или неудачного) задания печати, используемого для создания отчетов. Это не активное задание печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d4bd76dc84ad41c6d412144d13a784bec4f6a9f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050131"
---
# <a name="archivedprintjob-resource-type"></a><span data-ttu-id="e3a76-104">Тип ресурса Арчиведпринтжоб</span><span class="sxs-lookup"><span data-stu-id="e3a76-104">archivedPrintJob resource type</span></span>

<span data-ttu-id="e3a76-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3a76-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3a76-106">Запись "конечного состояния" (выполненного, прерванного или неудачного) задания печати, используемого для создания отчетов.</span><span class="sxs-lookup"><span data-stu-id="e3a76-106">A record of a "final state" (completed, aborted or failed) print job that is used for reporting purposes.</span></span> <span data-ttu-id="e3a76-107">Это не активное задание печати.</span><span class="sxs-lookup"><span data-stu-id="e3a76-107">This is not an active print job.</span></span>

## <a name="properties"></a><span data-ttu-id="e3a76-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3a76-108">Properties</span></span>
| <span data-ttu-id="e3a76-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3a76-109">Property</span></span>     | <span data-ttu-id="e3a76-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e3a76-110">Type</span></span>        | <span data-ttu-id="e3a76-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e3a76-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3a76-112">id</span><span class="sxs-lookup"><span data-stu-id="e3a76-112">id</span></span>|<span data-ttu-id="e3a76-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e3a76-113">String</span></span>|<span data-ttu-id="e3a76-114">Глобальный уникальный идентификатор (GUID) задания печати.</span><span class="sxs-lookup"><span data-stu-id="e3a76-114">The archived print job's GUID.</span></span> <span data-ttu-id="e3a76-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-115">Read-only.</span></span>|
|<span data-ttu-id="e3a76-116">принтерид</span><span class="sxs-lookup"><span data-stu-id="e3a76-116">printerId</span></span>|<span data-ttu-id="e3a76-117">Строка</span><span class="sxs-lookup"><span data-stu-id="e3a76-117">String</span></span>|<span data-ttu-id="e3a76-118">ИДЕНТИФИКАТОР принтера, для которого было задано задание в очереди.</span><span class="sxs-lookup"><span data-stu-id="e3a76-118">The printer ID that the job was queued for.</span></span> <span data-ttu-id="e3a76-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-119">Read-only.</span></span>|
|<span data-ttu-id="e3a76-120">процессингстате</span><span class="sxs-lookup"><span data-stu-id="e3a76-120">processingState</span></span>|<span data-ttu-id="e3a76-121">принтжобпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="e3a76-121">printJobProcessingState</span></span>|<span data-ttu-id="e3a76-122">Последнее состояние обработки задания печати.</span><span class="sxs-lookup"><span data-stu-id="e3a76-122">The print job's final processing state.</span></span> <span data-ttu-id="e3a76-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-123">Read-only.</span></span>|
|<span data-ttu-id="e3a76-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3a76-124">createdDateTime</span></span>|<span data-ttu-id="e3a76-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3a76-125">DateTimeOffset</span></span>|<span data-ttu-id="e3a76-126">Значение dateTimeOffset при создании задания.</span><span class="sxs-lookup"><span data-stu-id="e3a76-126">The dateTimeOffset when the job was created.</span></span> <span data-ttu-id="e3a76-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-127">Read-only.</span></span>|
|<span data-ttu-id="e3a76-128">аккуиреддатетиме</span><span class="sxs-lookup"><span data-stu-id="e3a76-128">acquiredDateTime</span></span>|<span data-ttu-id="e3a76-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3a76-129">DateTimeOffset</span></span>|<span data-ttu-id="e3a76-130">Значение dateTimeOffset, когда задание было получено принтером (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="e3a76-130">The dateTimeOffset when the job was acquired by the printer, if any.</span></span> <span data-ttu-id="e3a76-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-131">Read-only.</span></span>|
|<span data-ttu-id="e3a76-132">комплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="e3a76-132">completionDateTime</span></span>|<span data-ttu-id="e3a76-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3a76-133">DateTimeOffset</span></span>|<span data-ttu-id="e3a76-134">Значение dateTimeOffset, когда задание было завершено, отменено или прервано.</span><span class="sxs-lookup"><span data-stu-id="e3a76-134">The dateTimeOffset when the job was completed, canceled or aborted.</span></span> <span data-ttu-id="e3a76-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-135">Read-only.</span></span>|
|<span data-ttu-id="e3a76-136">аккуиредбипринтер</span><span class="sxs-lookup"><span data-stu-id="e3a76-136">acquiredByPrinter</span></span>|<span data-ttu-id="e3a76-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3a76-137">Boolean</span></span>|<span data-ttu-id="e3a76-138">Значение true, если задание было приобретено принтером; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="e3a76-138">True if the job was acquired by a printer; false otherwise.</span></span> <span data-ttu-id="e3a76-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-139">Read-only.</span></span>|
|<span data-ttu-id="e3a76-140">копиеспринтед</span><span class="sxs-lookup"><span data-stu-id="e3a76-140">copiesPrinted</span></span>|<span data-ttu-id="e3a76-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a76-141">Int32</span></span>|<span data-ttu-id="e3a76-142">Число напечатанных копий.</span><span class="sxs-lookup"><span data-stu-id="e3a76-142">The number of copies that were printed.</span></span> <span data-ttu-id="e3a76-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-143">Read-only.</span></span>|
|<span data-ttu-id="e3a76-144">pageCount</span><span class="sxs-lookup"><span data-stu-id="e3a76-144">pageCount</span></span>|<span data-ttu-id="e3a76-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a76-145">Int32</span></span>|<span data-ttu-id="e3a76-146">Общее количество напечатанных страниц.</span><span class="sxs-lookup"><span data-stu-id="e3a76-146">The total number of pages that were printed.</span></span> <span data-ttu-id="e3a76-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-147">Read-only.</span></span>|
|<span data-ttu-id="e3a76-148">блаккандвхитепажекаунт</span><span class="sxs-lookup"><span data-stu-id="e3a76-148">blackAndWhitePageCount</span></span>|<span data-ttu-id="e3a76-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a76-149">Int32</span></span>|<span data-ttu-id="e3a76-150">Количество напечатанных черно-белых страниц.</span><span class="sxs-lookup"><span data-stu-id="e3a76-150">The number of black and white pages that were printed.</span></span> <span data-ttu-id="e3a76-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-151">Read-only.</span></span>|
|<span data-ttu-id="e3a76-152">колорпажекаунт</span><span class="sxs-lookup"><span data-stu-id="e3a76-152">colorPageCount</span></span>|<span data-ttu-id="e3a76-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a76-153">Int32</span></span>|<span data-ttu-id="e3a76-154">Число напечатанных страниц цветов.</span><span class="sxs-lookup"><span data-stu-id="e3a76-154">The number of color pages that were printed.</span></span> <span data-ttu-id="e3a76-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-155">Read-only.</span></span>|
|<span data-ttu-id="e3a76-156">симплекспажекаунт</span><span class="sxs-lookup"><span data-stu-id="e3a76-156">simplexPageCount</span></span>|<span data-ttu-id="e3a76-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a76-157">Int32</span></span>|<span data-ttu-id="e3a76-158">Число напечатанных страниц симплекс (односторонняя).</span><span class="sxs-lookup"><span data-stu-id="e3a76-158">The number of simplex (single-sided) pages that were printed.</span></span> <span data-ttu-id="e3a76-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-159">Read-only.</span></span>|
|<span data-ttu-id="e3a76-160">дуплекспажекаунт</span><span class="sxs-lookup"><span data-stu-id="e3a76-160">duplexPageCount</span></span>|<span data-ttu-id="e3a76-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a76-161">Int32</span></span>|<span data-ttu-id="e3a76-162">Число отпечатанных дуплексных страниц (двусторонних).</span><span class="sxs-lookup"><span data-stu-id="e3a76-162">The number of duplex (double-sided) pages that were printed.</span></span> <span data-ttu-id="e3a76-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-163">Read-only.</span></span>|
|<span data-ttu-id="e3a76-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="e3a76-164">createdBy</span></span>|[<span data-ttu-id="e3a76-165">userIdentity</span><span class="sxs-lookup"><span data-stu-id="e3a76-165">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="e3a76-166">Пользователь, создавший задание печати.</span><span class="sxs-lookup"><span data-stu-id="e3a76-166">The user who created the print job.</span></span> <span data-ttu-id="e3a76-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3a76-167">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3a76-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3a76-168">JSON representation</span></span>

<span data-ttu-id="e3a76-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3a76-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->

```json
{
    "id": "String (identifier)",
    "printer": {"@odata.type": "microsoft.graph.directoryObject"},
    "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
    "processingState": {"@odata.type": "microsoft.graph.printJobProcessingState"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "archivedPrintJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

