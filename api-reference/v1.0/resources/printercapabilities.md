---
title: тип printerCapabilities сложный
description: Представляет возможности, сообщаемые принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bda913275aff692df2f66472f61436665cbc3dd7
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944228"
---
# <a name="printercapabilities-resource-type"></a><span data-ttu-id="26b77-103">тип ресурса printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="26b77-103">printerCapabilities resource type</span></span>

<span data-ttu-id="26b77-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="26b77-105">Представляет возможности, сообщаемые принтером или принтеромShare.</span><span class="sxs-lookup"><span data-stu-id="26b77-105">Represents the capabilities reported by a printer/printerShare.</span></span>

## <a name="properties"></a><span data-ttu-id="26b77-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="26b77-106">Properties</span></span>
| <span data-ttu-id="26b77-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="26b77-107">Property</span></span>     | <span data-ttu-id="26b77-108">Тип</span><span class="sxs-lookup"><span data-stu-id="26b77-108">Type</span></span>        | <span data-ttu-id="26b77-109">Описание</span><span class="sxs-lookup"><span data-stu-id="26b77-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26b77-110">contentTypes</span><span class="sxs-lookup"><span data-stu-id="26b77-110">contentTypes</span></span>|<span data-ttu-id="26b77-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="26b77-111">String collection</span></span>|<span data-ttu-id="26b77-112">Список поддерживаемых типов контента (MIME), поддерживаемых принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-112">A list of supported content (MIME) types that the printer supports.</span></span> <span data-ttu-id="26b77-113">Не гарантируется, что служба универсальной печати поддерживает печать всех этих типов MIME.</span><span class="sxs-lookup"><span data-stu-id="26b77-113">It is not guaranteed that the Universal Print service supports printing all of these MIME types.</span></span>|
|<span data-ttu-id="26b77-114">isColorPrintingSupported</span><span class="sxs-lookup"><span data-stu-id="26b77-114">isColorPrintingSupported</span></span>|<span data-ttu-id="26b77-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b77-115">Boolean</span></span>|<span data-ttu-id="26b77-116">True, если цветная печать поддерживается принтером; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="26b77-116">True if color printing is supported by the printer; false otherwise.</span></span> <span data-ttu-id="26b77-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="26b77-117">Read-only.</span></span>|
|<span data-ttu-id="26b77-118">feedOrientations</span><span class="sxs-lookup"><span data-stu-id="26b77-118">feedOrientations</span></span>|<span data-ttu-id="26b77-119">коллекция printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="26b77-119">printerFeedOrientation collection</span></span>|<span data-ttu-id="26b77-120">Список ориентаций каналов, поддерживаемых принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-120">The list of feed orientations that are supported by the printer.</span></span>|
|<span data-ttu-id="26b77-121">isPageRangeSupported</span><span class="sxs-lookup"><span data-stu-id="26b77-121">isPageRangeSupported</span></span>|<span data-ttu-id="26b77-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b77-122">Boolean</span></span>|<span data-ttu-id="26b77-123">True, если принтер поддерживает печать по диапазонам страниц; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="26b77-123">True if the printer supports printing by page ranges; false otherwise.</span></span>|
|<span data-ttu-id="26b77-124">качества</span><span class="sxs-lookup"><span data-stu-id="26b77-124">qualities</span></span>|<span data-ttu-id="26b77-125">[коллекция printQuality](enums.md#printquality-values)</span><span class="sxs-lookup"><span data-stu-id="26b77-125">[printQuality](enums.md#printquality-values) collection</span></span>|<span data-ttu-id="26b77-126">Свойства печати, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-126">The print qualities supported by the printer.</span></span>|
|<span data-ttu-id="26b77-127">dpis</span><span class="sxs-lookup"><span data-stu-id="26b77-127">dpis</span></span>|<span data-ttu-id="26b77-128">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="26b77-128">Int32 collection</span></span>|<span data-ttu-id="26b77-129">Список разрешений печати в DPI, поддерживаемых принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-129">The list of print resolutions in DPI that are supported by the printer.</span></span>|
|<span data-ttu-id="26b77-130">duplexModes</span><span class="sxs-lookup"><span data-stu-id="26b77-130">duplexModes</span></span>|<span data-ttu-id="26b77-131">[коллекция printDuplexMode](enums.md#printduplexmode-values)</span><span class="sxs-lookup"><span data-stu-id="26b77-131">[printDuplexMode](enums.md#printduplexmode-values) collection</span></span>|<span data-ttu-id="26b77-132">Список режимов дуплекса, поддерживаемых принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-132">The list of duplex modes that are supported by the printer.</span></span> <span data-ttu-id="26b77-133">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="26b77-133">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="26b77-134">queueBufferSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="26b77-134">queueBufferSizeInBytes</span></span>|<span data-ttu-id="26b77-135">Int32</span><span class="sxs-lookup"><span data-stu-id="26b77-135">Int32</span></span>|<span data-ttu-id="26b77-136">Максимальный размер очереди задания печати, который может храниться на принтере.</span><span class="sxs-lookup"><span data-stu-id="26b77-136">The maximum print job queue size that can be stored by the printer.</span></span>|
|<span data-ttu-id="26b77-137">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="26b77-137">copiesPerJob</span></span>|[<span data-ttu-id="26b77-138">integerRange</span><span class="sxs-lookup"><span data-stu-id="26b77-138">integerRange</span></span>](integerrange.md)|<span data-ttu-id="26b77-139">Диапазон копий на одну работу, поддерживаемую принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-139">The range of copies per job supported by the printer.</span></span>|
|<span data-ttu-id="26b77-140">finishings</span><span class="sxs-lookup"><span data-stu-id="26b77-140">finishings</span></span>|<span data-ttu-id="26b77-141">[коллекция printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="26b77-141">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="26b77-142">Отделочные процессы, поддерживаемые принтером для печатного документа.</span><span class="sxs-lookup"><span data-stu-id="26b77-142">Finishing processes the printer supports for a printed document.</span></span>|
|<span data-ttu-id="26b77-143">mediaColors</span><span class="sxs-lookup"><span data-stu-id="26b77-143">mediaColors</span></span>|<span data-ttu-id="26b77-144">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="26b77-144">String collection</span></span>|<span data-ttu-id="26b77-145">Средства массовой информации (например, бумажные) цвета, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-145">The media (i.e., paper) colors supported by the printer.</span></span>|
|<span data-ttu-id="26b77-146">mediaTypes</span><span class="sxs-lookup"><span data-stu-id="26b77-146">mediaTypes</span></span>|<span data-ttu-id="26b77-147">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="26b77-147">String collection</span></span>|<span data-ttu-id="26b77-148">Типы мультимедиа, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-148">The media types supported by the printer.</span></span>|
|<span data-ttu-id="26b77-149">mediaSizes</span><span class="sxs-lookup"><span data-stu-id="26b77-149">mediaSizes</span></span>|<span data-ttu-id="26b77-150">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="26b77-150">String collection</span></span>|<span data-ttu-id="26b77-151">Размеры мультимедиа, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-151">The media sizes supported by the printer.</span></span> <span data-ttu-id="26b77-152">Поддерживает стандартные имена размеров для средств массовой информации ISO и ANSI.</span><span class="sxs-lookup"><span data-stu-id="26b77-152">Supports standard size names for ISO and ANSI media sizes.</span></span> <span data-ttu-id="26b77-153">Допустимые значения находятся в следующей [таблице.](#mediasizes-values)</span><span class="sxs-lookup"><span data-stu-id="26b77-153">Valid values are in the following [table](#mediasizes-values).</span></span>|
|<span data-ttu-id="26b77-154">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="26b77-154">pagesPerSheet</span></span>|<span data-ttu-id="26b77-155">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="26b77-155">Int32 collection</span></span>|<span data-ttu-id="26b77-156">Поддерживаемое количество страниц ввода, которые необходимо навязать одному впечатлению.</span><span class="sxs-lookup"><span data-stu-id="26b77-156">Supported number of Input Pages to impose upon a single Impression.</span></span>|
|<span data-ttu-id="26b77-157">ориентации</span><span class="sxs-lookup"><span data-stu-id="26b77-157">orientations</span></span>|<span data-ttu-id="26b77-158">[коллекция printOrientation](enums.md#printorientation-values)</span><span class="sxs-lookup"><span data-stu-id="26b77-158">[printOrientation](enums.md#printorientation-values) collection</span></span>|<span data-ttu-id="26b77-159">Ориентации печати, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-159">The print orientations supported by the printer.</span></span> <span data-ttu-id="26b77-160">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="26b77-160">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="26b77-161">inputBins</span><span class="sxs-lookup"><span data-stu-id="26b77-161">inputBins</span></span>|<span data-ttu-id="26b77-162">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="26b77-162">String collection</span></span>|<span data-ttu-id="26b77-163">Поддерживаемые ячейки ввода для принтера.</span><span class="sxs-lookup"><span data-stu-id="26b77-163">Supported input bins for the printer.</span></span>|
|<span data-ttu-id="26b77-164">outputBins</span><span class="sxs-lookup"><span data-stu-id="26b77-164">outputBins</span></span>|<span data-ttu-id="26b77-165">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="26b77-165">String collection</span></span>|<span data-ttu-id="26b77-166">Поддерживаемые ячейки вывода принтера (лотки).</span><span class="sxs-lookup"><span data-stu-id="26b77-166">The printer's supported output bins (trays).</span></span>|
|<span data-ttu-id="26b77-167">supportsFitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="26b77-167">supportsFitPdfToPage</span></span>|<span data-ttu-id="26b77-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b77-168">Boolean</span></span>|<span data-ttu-id="26b77-169">True, если принтер поддерживает масштабирование страниц PDF в соответствие с размером печатных мультимедиа; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="26b77-169">True if the printer supports scaling PDF pages to match the print media size; false otherwise.</span></span>|
|<span data-ttu-id="26b77-170">multipageLayouts</span><span class="sxs-lookup"><span data-stu-id="26b77-170">multipageLayouts</span></span>|<span data-ttu-id="26b77-171">[коллекция printMultipageLayout](enums.md#printmultipagelayout-values)</span><span class="sxs-lookup"><span data-stu-id="26b77-171">[printMultipageLayout](enums.md#printmultipagelayout-values) collection</span></span>|<span data-ttu-id="26b77-172">Направления презентации, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-172">The presentation directions supported by the printer.</span></span> <span data-ttu-id="26b77-173">Поддерживаемые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="26b77-173">Supported values are described in the following table.</span></span>|
|<span data-ttu-id="26b77-174">colorModes</span><span class="sxs-lookup"><span data-stu-id="26b77-174">colorModes</span></span>|<span data-ttu-id="26b77-175">[коллекция printColorMode](enums.md#printcolormode-values)</span><span class="sxs-lookup"><span data-stu-id="26b77-175">[printColorMode](enums.md#printcolormode-values) collection</span></span>|<span data-ttu-id="26b77-176">Цветовые режимы, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="26b77-176">The color modes supported by the printer.</span></span> <span data-ttu-id="26b77-177">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="26b77-177">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="26b77-178">topMargins</span><span class="sxs-lookup"><span data-stu-id="26b77-178">topMargins</span></span>|<span data-ttu-id="26b77-179">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="26b77-179">Int32 collection</span></span>|<span data-ttu-id="26b77-180">Список поддерживаемых верхних полей (в микронах) для принтера.</span><span class="sxs-lookup"><span data-stu-id="26b77-180">A list of supported top margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="26b77-181">bottomMargins</span><span class="sxs-lookup"><span data-stu-id="26b77-181">bottomMargins</span></span>|<span data-ttu-id="26b77-182">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="26b77-182">Int32 collection</span></span>|<span data-ttu-id="26b77-183">Список поддерживаемых нижних полей (в микронах) для принтера.</span><span class="sxs-lookup"><span data-stu-id="26b77-183">A list of supported bottom margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="26b77-184">rightMargins</span><span class="sxs-lookup"><span data-stu-id="26b77-184">rightMargins</span></span>|<span data-ttu-id="26b77-185">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="26b77-185">Int32 collection</span></span>|<span data-ttu-id="26b77-186">Список поддерживаемых правых полей (в микронах) для принтера.</span><span class="sxs-lookup"><span data-stu-id="26b77-186">A list of supported right margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="26b77-187">leftMargins</span><span class="sxs-lookup"><span data-stu-id="26b77-187">leftMargins</span></span>|<span data-ttu-id="26b77-188">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="26b77-188">Int32 collection</span></span>|<span data-ttu-id="26b77-189">Список поддерживаемых левых полей (в микронах) для принтера.</span><span class="sxs-lookup"><span data-stu-id="26b77-189">A list of supported left margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="26b77-190">collation</span><span class="sxs-lookup"><span data-stu-id="26b77-190">collation</span></span>|<span data-ttu-id="26b77-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="26b77-191">Boolean</span></span>|<span data-ttu-id="26b77-192">True, если принтер поддерживает копирование при печати muliple копий многошагового документа; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="26b77-192">True if the printer supports collating when printing muliple copies of a multi-page document; false otherwise.</span></span>|
|<span data-ttu-id="26b77-193">scalings</span><span class="sxs-lookup"><span data-stu-id="26b77-193">scalings</span></span>|<span data-ttu-id="26b77-194">[коллекция printScaling](enums.md#printscaling-values)</span><span class="sxs-lookup"><span data-stu-id="26b77-194">[printScaling](enums.md#printscaling-values) collection</span></span>|<span data-ttu-id="26b77-195">Поддерживаемые масштабирования печати.</span><span class="sxs-lookup"><span data-stu-id="26b77-195">Supported print scalings.</span></span>|

### <a name="mediasizes-values"></a><span data-ttu-id="26b77-196">mediaSizes values</span><span class="sxs-lookup"><span data-stu-id="26b77-196">mediaSizes values</span></span>

|<span data-ttu-id="26b77-197">Значение</span><span class="sxs-lookup"><span data-stu-id="26b77-197">Value</span></span>|
|:---|
|<span data-ttu-id="26b77-198">A3</span><span class="sxs-lookup"><span data-stu-id="26b77-198">A3</span></span>|
|<span data-ttu-id="26b77-199">A4</span><span class="sxs-lookup"><span data-stu-id="26b77-199">A4</span></span>|
|<span data-ttu-id="26b77-200">A5</span><span class="sxs-lookup"><span data-stu-id="26b77-200">A5</span></span>|
|<span data-ttu-id="26b77-201">A6</span><span class="sxs-lookup"><span data-stu-id="26b77-201">A6</span></span>|
|<span data-ttu-id="26b77-202">JIS B4</span><span class="sxs-lookup"><span data-stu-id="26b77-202">JIS B4</span></span>|
|<span data-ttu-id="26b77-203">JIS B5</span><span class="sxs-lookup"><span data-stu-id="26b77-203">JIS B5</span></span>|
|<span data-ttu-id="26b77-204">JPN Hagaki</span><span class="sxs-lookup"><span data-stu-id="26b77-204">JPN Hagaki</span></span>|
|<span data-ttu-id="26b77-205">Северная Америка 5x7in</span><span class="sxs-lookup"><span data-stu-id="26b77-205">North America 5x7in</span></span>|
|<span data-ttu-id="26b77-206">Северная Америка Executive</span><span class="sxs-lookup"><span data-stu-id="26b77-206">North America Executive</span></span>|
|<span data-ttu-id="26b77-207">Письмо говермента Северной Америки</span><span class="sxs-lookup"><span data-stu-id="26b77-207">North America Goverment Letter</span></span>|
|<span data-ttu-id="26b77-208">Индекс Северной Америки 3x5in</span><span class="sxs-lookup"><span data-stu-id="26b77-208">North America Index 3x5in</span></span>|
|<span data-ttu-id="26b77-209">Индекс Северной Америки 4x8in</span><span class="sxs-lookup"><span data-stu-id="26b77-209">North America Index 4x8in</span></span>|
|<span data-ttu-id="26b77-210">Индекс Северной Америки 5x8in</span><span class="sxs-lookup"><span data-stu-id="26b77-210">North America Index 5x8in</span></span>|
|<span data-ttu-id="26b77-211">Счет в Северной Америке</span><span class="sxs-lookup"><span data-stu-id="26b77-211">North America Invoice</span></span>|
|<span data-ttu-id="26b77-212">Книги Северной Америки</span><span class="sxs-lookup"><span data-stu-id="26b77-212">North America Ledger</span></span>|
|<span data-ttu-id="26b77-213">Северная Америка Legal</span><span class="sxs-lookup"><span data-stu-id="26b77-213">North America Legal</span></span>|
|<span data-ttu-id="26b77-214">Письмо Из Северной Америки</span><span class="sxs-lookup"><span data-stu-id="26b77-214">North America Letter</span></span>|
|<span data-ttu-id="26b77-215">Фото l 3.5x5in</span><span class="sxs-lookup"><span data-stu-id="26b77-215">Photo l 3.5x5in</span></span>|
|<span data-ttu-id="26b77-216">Визитная карточка</span><span class="sxs-lookup"><span data-stu-id="26b77-216">Business Card</span></span>|
|<span data-ttu-id="26b77-217">Photo</span><span class="sxs-lookup"><span data-stu-id="26b77-217">Photo</span></span>|

## <a name="relationships"></a><span data-ttu-id="26b77-218">Связи</span><span class="sxs-lookup"><span data-stu-id="26b77-218">Relationships</span></span>
<span data-ttu-id="26b77-219">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="26b77-219">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26b77-220">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="26b77-220">JSON representation</span></span>
<span data-ttu-id="26b77-221">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26b77-221">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerCapabilities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCapabilities",
  "contentTypes": [
    "String"
  ],
  "isColorPrintingSupported": "Boolean",
  "feedOrientations": [
    "String"
  ],
  "isPageRangeSupported": "Boolean",
  "qualities": [
    "String"
  ],
  "dpis": [
    "Integer"
  ],
  "duplexModes": [
    "String"
  ],
  "copiesPerJob": {
    "@odata.type": "microsoft.graph.integerRange"
  },
  "finishings": [
    "String"
  ],
  "mediaColors": [
    "String"
  ],
  "mediaTypes": [
    "String"
  ],
  "mediaSizes": [
    "String"
  ],
  "pagesPerSheet": [
    "Integer"
  ],
  "orientations": [
    "String"
  ],
  "outputBins": [
    "String"
  ],
  "supportsFitPdfToPage": "Boolean",
  "multipageLayouts": [
    "String"
  ],
  "colorModes": [
    "String"
  ],
  "inputBins": [
    "String"
  ],
  "topMargins": [
    "Integer"
  ],
  "bottomMargins": [
    "Integer"
  ],
  "rightMargins": [
    "Integer"
  ],
  "leftMargins": [
    "Integer"
  ],
  "collation": "Boolean",
  "scalings": [
    "String"
  ]
}
```

