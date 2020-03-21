---
title: Тип ресурса Арчиведпринтжоб
description: Запись "конечного состояния" (выполненного, прерванного или неудачного) задания печати, используемого для создания отчетов. Это не активное задание печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 170f3b735b4f14173058efbaaa1c81b80490f020
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895993"
---
# <a name="archivedprintjob-resource-type"></a><span data-ttu-id="6f38b-104">Тип ресурса Арчиведпринтжоб</span><span class="sxs-lookup"><span data-stu-id="6f38b-104">archivedPrintJob resource type</span></span>

<span data-ttu-id="6f38b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f38b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f38b-106">Запись "конечного состояния" (выполненного, прерванного или неудачного) задания печати, используемого для создания отчетов.</span><span class="sxs-lookup"><span data-stu-id="6f38b-106">A record of a "final state" (completed, aborted or failed) print job that is used for reporting purposes.</span></span> <span data-ttu-id="6f38b-107">Это не активное задание печати.</span><span class="sxs-lookup"><span data-stu-id="6f38b-107">This is not an active print job.</span></span>

## <a name="properties"></a><span data-ttu-id="6f38b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f38b-108">Properties</span></span>
| <span data-ttu-id="6f38b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f38b-109">Property</span></span>     | <span data-ttu-id="6f38b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6f38b-110">Type</span></span>        | <span data-ttu-id="6f38b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6f38b-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f38b-112">id</span><span class="sxs-lookup"><span data-stu-id="6f38b-112">id</span></span>|<span data-ttu-id="6f38b-113">String</span><span class="sxs-lookup"><span data-stu-id="6f38b-113">String</span></span>|<span data-ttu-id="6f38b-114">Глобальный уникальный идентификатор (GUID) задания печати.</span><span class="sxs-lookup"><span data-stu-id="6f38b-114">The archived print job's GUID.</span></span> <span data-ttu-id="6f38b-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-115">Read-only.</span></span>|
|<span data-ttu-id="6f38b-116">принтерид</span><span class="sxs-lookup"><span data-stu-id="6f38b-116">printerId</span></span>|<span data-ttu-id="6f38b-117">String</span><span class="sxs-lookup"><span data-stu-id="6f38b-117">String</span></span>|<span data-ttu-id="6f38b-118">ИДЕНТИФИКАТОР принтера, для которого было задано задание в очереди.</span><span class="sxs-lookup"><span data-stu-id="6f38b-118">The printer ID that the job was queued for.</span></span> <span data-ttu-id="6f38b-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-119">Read-only.</span></span>|
|<span data-ttu-id="6f38b-120">процессингстате</span><span class="sxs-lookup"><span data-stu-id="6f38b-120">processingState</span></span>|<span data-ttu-id="6f38b-121">принтжобпроцессингстате</span><span class="sxs-lookup"><span data-stu-id="6f38b-121">printJobProcessingState</span></span>|<span data-ttu-id="6f38b-122">Последнее состояние обработки задания печати.</span><span class="sxs-lookup"><span data-stu-id="6f38b-122">The print job's final processing state.</span></span> <span data-ttu-id="6f38b-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-123">Read-only.</span></span>|
|<span data-ttu-id="6f38b-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f38b-124">createdDateTime</span></span>|<span data-ttu-id="6f38b-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f38b-125">DateTimeOffset</span></span>|<span data-ttu-id="6f38b-126">Значение dateTimeOffset при создании задания.</span><span class="sxs-lookup"><span data-stu-id="6f38b-126">The dateTimeOffset when the job was created.</span></span> <span data-ttu-id="6f38b-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-127">Read-only.</span></span>|
|<span data-ttu-id="6f38b-128">аккуиреддатетиме</span><span class="sxs-lookup"><span data-stu-id="6f38b-128">acquiredDateTime</span></span>|<span data-ttu-id="6f38b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f38b-129">DateTimeOffset</span></span>|<span data-ttu-id="6f38b-130">Значение dateTimeOffset, когда задание было получено принтером (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="6f38b-130">The dateTimeOffset when the job was acquired by the printer, if any.</span></span> <span data-ttu-id="6f38b-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-131">Read-only.</span></span>|
|<span data-ttu-id="6f38b-132">комплетиондатетиме</span><span class="sxs-lookup"><span data-stu-id="6f38b-132">completionDateTime</span></span>|<span data-ttu-id="6f38b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f38b-133">DateTimeOffset</span></span>|<span data-ttu-id="6f38b-134">Значение dateTimeOffset, когда задание было завершено, отменено или прервано.</span><span class="sxs-lookup"><span data-stu-id="6f38b-134">The dateTimeOffset when the job was completed, canceled or aborted.</span></span> <span data-ttu-id="6f38b-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-135">Read-only.</span></span>|
|<span data-ttu-id="6f38b-136">аккуиредбипринтер</span><span class="sxs-lookup"><span data-stu-id="6f38b-136">acquiredByPrinter</span></span>|<span data-ttu-id="6f38b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f38b-137">Boolean</span></span>|<span data-ttu-id="6f38b-138">Значение true, если задание было приобретено принтером; в противном случае — false.</span><span class="sxs-lookup"><span data-stu-id="6f38b-138">True if the job was acquired by a printer; false otherwise.</span></span> <span data-ttu-id="6f38b-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-139">Read-only.</span></span>|
|<span data-ttu-id="6f38b-140">копиеспринтед</span><span class="sxs-lookup"><span data-stu-id="6f38b-140">copiesPrinted</span></span>|<span data-ttu-id="6f38b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6f38b-141">Int32</span></span>|<span data-ttu-id="6f38b-142">Число напечатанных копий.</span><span class="sxs-lookup"><span data-stu-id="6f38b-142">The number of copies that were printed.</span></span> <span data-ttu-id="6f38b-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-143">Read-only.</span></span>|
|<span data-ttu-id="6f38b-144">pageCount</span><span class="sxs-lookup"><span data-stu-id="6f38b-144">pageCount</span></span>|<span data-ttu-id="6f38b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6f38b-145">Int32</span></span>|<span data-ttu-id="6f38b-146">Общее количество напечатанных страниц.</span><span class="sxs-lookup"><span data-stu-id="6f38b-146">The total number of pages that were printed.</span></span> <span data-ttu-id="6f38b-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-147">Read-only.</span></span>|
|<span data-ttu-id="6f38b-148">блаккандвхитепажекаунт</span><span class="sxs-lookup"><span data-stu-id="6f38b-148">blackAndWhitePageCount</span></span>|<span data-ttu-id="6f38b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6f38b-149">Int32</span></span>|<span data-ttu-id="6f38b-150">Количество напечатанных черно-белых страниц.</span><span class="sxs-lookup"><span data-stu-id="6f38b-150">The number of black and white pages that were printed.</span></span> <span data-ttu-id="6f38b-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-151">Read-only.</span></span>|
|<span data-ttu-id="6f38b-152">колорпажекаунт</span><span class="sxs-lookup"><span data-stu-id="6f38b-152">colorPageCount</span></span>|<span data-ttu-id="6f38b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6f38b-153">Int32</span></span>|<span data-ttu-id="6f38b-154">Число напечатанных страниц цветов.</span><span class="sxs-lookup"><span data-stu-id="6f38b-154">The number of color pages that were printed.</span></span> <span data-ttu-id="6f38b-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-155">Read-only.</span></span>|
|<span data-ttu-id="6f38b-156">симплекспажекаунт</span><span class="sxs-lookup"><span data-stu-id="6f38b-156">simplexPageCount</span></span>|<span data-ttu-id="6f38b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6f38b-157">Int32</span></span>|<span data-ttu-id="6f38b-158">Число напечатанных страниц симплекс (односторонняя).</span><span class="sxs-lookup"><span data-stu-id="6f38b-158">The number of simplex (single-sided) pages that were printed.</span></span> <span data-ttu-id="6f38b-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-159">Read-only.</span></span>|
|<span data-ttu-id="6f38b-160">дуплекспажекаунт</span><span class="sxs-lookup"><span data-stu-id="6f38b-160">duplexPageCount</span></span>|<span data-ttu-id="6f38b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="6f38b-161">Int32</span></span>|<span data-ttu-id="6f38b-162">Число отпечатанных дуплексных страниц (двусторонних).</span><span class="sxs-lookup"><span data-stu-id="6f38b-162">The number of duplex (double-sided) pages that were printed.</span></span> <span data-ttu-id="6f38b-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-163">Read-only.</span></span>|
|<span data-ttu-id="6f38b-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="6f38b-164">createdBy</span></span>|[<span data-ttu-id="6f38b-165">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6f38b-165">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="6f38b-166">Пользователь, создавший задание печати.</span><span class="sxs-lookup"><span data-stu-id="6f38b-166">The user who created the print job.</span></span> <span data-ttu-id="6f38b-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f38b-167">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f38b-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f38b-168">JSON representation</span></span>

<span data-ttu-id="6f38b-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f38b-169">The following is a JSON representation of the resource.</span></span>

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