---
title: тип ресурса printerDefaults
description: Представляет параметры принтера по умолчанию. Проверьте возможности принтера, чтобы увидеть все поддерживаемые значения.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fbee453d42fbcb056ce3dce3ff7311e4d976b7dc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517343"
---
# <a name="printerdefaults-resource-type"></a><span data-ttu-id="a1ace-104">тип ресурса printerDefaults</span><span class="sxs-lookup"><span data-stu-id="a1ace-104">printerDefaults resource type</span></span>

<span data-ttu-id="a1ace-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1ace-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a1ace-106">Представляет параметры принтера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1ace-106">Represents the printer's default settings.</span></span> <span data-ttu-id="a1ace-107">Проверьте возможности [принтера,](printercapabilities.md) чтобы увидеть все поддерживаемые значения.</span><span class="sxs-lookup"><span data-stu-id="a1ace-107">Check the printer's [capabilities](printercapabilities.md) to see all the values that it supports.</span></span>

## <a name="properties"></a><span data-ttu-id="a1ace-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1ace-108">Properties</span></span>
|<span data-ttu-id="a1ace-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1ace-109">Property</span></span>|<span data-ttu-id="a1ace-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a1ace-110">Type</span></span>|<span data-ttu-id="a1ace-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a1ace-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ace-112">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="a1ace-112">copiesPerJob</span></span>|<span data-ttu-id="a1ace-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a1ace-113">Int32</span></span>|<span data-ttu-id="a1ace-114">Число экземпляров, напечатанных по умолчанию на одну работу.</span><span class="sxs-lookup"><span data-stu-id="a1ace-114">The default number of copies printed per job.</span></span>|
|<span data-ttu-id="a1ace-115">contentType</span><span class="sxs-lookup"><span data-stu-id="a1ace-115">contentType</span></span>|<span data-ttu-id="a1ace-116">String</span><span class="sxs-lookup"><span data-stu-id="a1ace-116">String</span></span>|<span data-ttu-id="a1ace-117">Тип контента по умолчанию (MIME), который используется при обработке документов.</span><span class="sxs-lookup"><span data-stu-id="a1ace-117">The default content (MIME) type to use when processing documents.</span></span>|
|<span data-ttu-id="a1ace-118">finishings</span><span class="sxs-lookup"><span data-stu-id="a1ace-118">finishings</span></span>|<span data-ttu-id="a1ace-119">[коллекция printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="a1ace-119">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="a1ace-120">Набор отделок по умолчанию, применимый к заданиям печати.</span><span class="sxs-lookup"><span data-stu-id="a1ace-120">The default set of finishings to apply to print jobs.</span></span> <span data-ttu-id="a1ace-121">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1ace-121">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a1ace-122">mediaColor</span><span class="sxs-lookup"><span data-stu-id="a1ace-122">mediaColor</span></span>|<span data-ttu-id="a1ace-123">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ace-123">String</span></span>|<span data-ttu-id="a1ace-124">Цвет мультимедиа по умолчанию (например, бумажный) для печати документа.</span><span class="sxs-lookup"><span data-stu-id="a1ace-124">The default media (such as paper) color to print the document on.</span></span>
|<span data-ttu-id="a1ace-125">MediaType</span><span class="sxs-lookup"><span data-stu-id="a1ace-125">mediaType</span></span>|<span data-ttu-id="a1ace-126">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ace-126">String</span></span>|<span data-ttu-id="a1ace-127">Тип мультимедиа по умолчанию (например, бумага) для печати документа.</span><span class="sxs-lookup"><span data-stu-id="a1ace-127">The default media (such as paper) type to print the document on.</span></span> <span data-ttu-id="a1ace-128">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1ace-128">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a1ace-129">mediaSize</span><span class="sxs-lookup"><span data-stu-id="a1ace-129">mediaSize</span></span>|<span data-ttu-id="a1ace-130">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ace-130">String</span></span>|<span data-ttu-id="a1ace-131">Размер мультимедиа по умолчанию, который необходимо использовать.</span><span class="sxs-lookup"><span data-stu-id="a1ace-131">The default media size to use.</span></span> <span data-ttu-id="a1ace-132">Поддерживает стандартные имена размеров для средств массовой информации ISO и ANSI, а также любые настраиваемые размеры, поддерживаемые связанным принтером.</span><span class="sxs-lookup"><span data-stu-id="a1ace-132">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>
|<span data-ttu-id="a1ace-133">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="a1ace-133">pagesPerSheet</span></span>|<span data-ttu-id="a1ace-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a1ace-134">Int32</span></span>|<span data-ttu-id="a1ace-135">Число страниц документов по умолчанию для печати на каждом листе.</span><span class="sxs-lookup"><span data-stu-id="a1ace-135">The default number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="a1ace-136">orientation</span><span class="sxs-lookup"><span data-stu-id="a1ace-136">orientation</span></span>|[<span data-ttu-id="a1ace-137">printOrientation</span><span class="sxs-lookup"><span data-stu-id="a1ace-137">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="a1ace-138">Ориентация по умолчанию, используемая при печати документа.</span><span class="sxs-lookup"><span data-stu-id="a1ace-138">The default orientation to use when printing the document.</span></span> <span data-ttu-id="a1ace-139">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1ace-139">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a1ace-140">outputBin</span><span class="sxs-lookup"><span data-stu-id="a1ace-140">outputBin</span></span>|<span data-ttu-id="a1ace-141">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ace-141">String</span></span>|<span data-ttu-id="a1ace-142">Ячейка вывода по умолчанию для того, чтобы разместить завершенные отпечатки.</span><span class="sxs-lookup"><span data-stu-id="a1ace-142">The default output bin to place completed prints into.</span></span> <span data-ttu-id="a1ace-143">См. возможности [принтера для](printercapabilities.md) списка поддерживаемых бункеров выходных данных.</span><span class="sxs-lookup"><span data-stu-id="a1ace-143">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="a1ace-144">fitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="a1ace-144">fitPdfToPage</span></span>|<span data-ttu-id="a1ace-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a1ace-145">Boolean</span></span>|<span data-ttu-id="a1ace-146">Параметр fitPdfToPage по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a1ace-146">The default fitPdfToPage setting.</span></span> <span data-ttu-id="a1ace-147">True, чтобы поместить каждую страницу документа PDF в физический лист мультимедиа; false, чтобы принтер решил, как выкладывать впечатления.</span><span class="sxs-lookup"><span data-stu-id="a1ace-147">True to fit each page of a PDF document to a physical sheet of media; false to let the printer decide how to lay out impressions.</span></span>|
|<span data-ttu-id="a1ace-148">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="a1ace-148">multipageLayout</span></span>|[<span data-ttu-id="a1ace-149">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="a1ace-149">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="a1ace-150">Направление по умолчанию для выкладки страниц при печати нескольких страниц на листе.</span><span class="sxs-lookup"><span data-stu-id="a1ace-150">The default direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="a1ace-151">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1ace-151">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a1ace-152">colorMode</span><span class="sxs-lookup"><span data-stu-id="a1ace-152">colorMode</span></span>|[<span data-ttu-id="a1ace-153">printColorMode</span><span class="sxs-lookup"><span data-stu-id="a1ace-153">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="a1ace-154">Цветной режим по умолчанию, который используется при печати документа.</span><span class="sxs-lookup"><span data-stu-id="a1ace-154">The default color mode to use when printing the document.</span></span> <span data-ttu-id="a1ace-155">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1ace-155">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a1ace-156">качество</span><span class="sxs-lookup"><span data-stu-id="a1ace-156">quality</span></span>|[<span data-ttu-id="a1ace-157">printQuality</span><span class="sxs-lookup"><span data-stu-id="a1ace-157">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="a1ace-158">Качество по умолчанию, используемая при печати документа.</span><span class="sxs-lookup"><span data-stu-id="a1ace-158">The default quality to use when printing the document.</span></span> <span data-ttu-id="a1ace-159">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1ace-159">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a1ace-160">duplexMode</span><span class="sxs-lookup"><span data-stu-id="a1ace-160">duplexMode</span></span>|[<span data-ttu-id="a1ace-161">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="a1ace-161">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="a1ace-162">Двубоксовая конфигурация по умолчанию, используемая при печати документа.</span><span class="sxs-lookup"><span data-stu-id="a1ace-162">The default duplex (double-sided) configuration to use when printing a document.</span></span> <span data-ttu-id="a1ace-163">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1ace-163">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a1ace-164">dpi</span><span class="sxs-lookup"><span data-stu-id="a1ace-164">dpi</span></span>|<span data-ttu-id="a1ace-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a1ace-165">Int32</span></span>|<span data-ttu-id="a1ace-166">Разрешение по умолчанию в DPI, используемом при печати задания.</span><span class="sxs-lookup"><span data-stu-id="a1ace-166">The default resolution in DPI to use when printing the job.</span></span>|
|<span data-ttu-id="a1ace-167">scaling</span><span class="sxs-lookup"><span data-stu-id="a1ace-167">scaling</span></span>|[<span data-ttu-id="a1ace-168">printScaling</span><span class="sxs-lookup"><span data-stu-id="a1ace-168">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="a1ace-169">Указывает, как принтер масштабирует данные документа, чтобы соответствовать запрашиваемой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="a1ace-169">Specifies how the printer scales the document data to fit the requested media.</span></span> <span data-ttu-id="a1ace-170">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1ace-170">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1ace-171">Отношения</span><span class="sxs-lookup"><span data-stu-id="a1ace-171">Relationships</span></span>
<span data-ttu-id="a1ace-172">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a1ace-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1ace-173">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a1ace-173">JSON representation</span></span>
<span data-ttu-id="a1ace-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1ace-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerDefaults"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerDefaults",
  "copiesPerJob": "Integer",
  "contentType": "String",
  "finishings": [
    "String"
  ],
  "mediaColor": "String",
  "mediaType": "String",
  "mediaSize": "String",
  "pagesPerSheet": "Integer",
  "orientation": "String",
  "outputBin": "String",
  "inputBin": "String",
  "fitPdfToPage": "Boolean",
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String",
  "dpi": "Integer",
  "scaling": "String"
}
```

