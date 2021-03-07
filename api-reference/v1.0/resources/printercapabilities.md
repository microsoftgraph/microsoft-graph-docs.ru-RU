---
title: тип printerCapabilities сложный
description: Представляет возможности, сообщаемые принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5416cf43e266bab65254ac5aaee1a79c9c3e17be
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517338"
---
# <a name="printercapabilities-resource-type"></a><span data-ttu-id="67e17-103">тип ресурса printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="67e17-103">printerCapabilities resource type</span></span>

<span data-ttu-id="67e17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67e17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="67e17-105">Представляет возможности, сообщаемые принтером или принтеромShare.</span><span class="sxs-lookup"><span data-stu-id="67e17-105">Represents the capabilities reported by a printer/printerShare.</span></span>

## <a name="properties"></a><span data-ttu-id="67e17-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="67e17-106">Properties</span></span>
| <span data-ttu-id="67e17-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="67e17-107">Property</span></span>     | <span data-ttu-id="67e17-108">Тип</span><span class="sxs-lookup"><span data-stu-id="67e17-108">Type</span></span>        | <span data-ttu-id="67e17-109">Описание</span><span class="sxs-lookup"><span data-stu-id="67e17-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67e17-110">contentTypes</span><span class="sxs-lookup"><span data-stu-id="67e17-110">contentTypes</span></span>|<span data-ttu-id="67e17-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67e17-111">String collection</span></span>|<span data-ttu-id="67e17-112">Список поддерживаемых типов контента (MIME), поддерживаемых принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-112">A list of supported content (MIME) types that the printer supports.</span></span> <span data-ttu-id="67e17-113">Не гарантируется, что служба универсальной печати поддерживает печать всех этих типов MIME.</span><span class="sxs-lookup"><span data-stu-id="67e17-113">It is not guaranteed that the Universal Print service supports printing all of these MIME types.</span></span>|
|<span data-ttu-id="67e17-114">isColorPrintingSupported</span><span class="sxs-lookup"><span data-stu-id="67e17-114">isColorPrintingSupported</span></span>|<span data-ttu-id="67e17-115">Логический</span><span class="sxs-lookup"><span data-stu-id="67e17-115">Boolean</span></span>|<span data-ttu-id="67e17-116">True, если цветная печать поддерживается принтером; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="67e17-116">True if color printing is supported by the printer; false otherwise.</span></span> <span data-ttu-id="67e17-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67e17-117">Read-only.</span></span>|
|<span data-ttu-id="67e17-118">feedOrientations</span><span class="sxs-lookup"><span data-stu-id="67e17-118">feedOrientations</span></span>|<span data-ttu-id="67e17-119">коллекция printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="67e17-119">printerFeedOrientation collection</span></span>|<span data-ttu-id="67e17-120">Список ориентаций каналов, поддерживаемых принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-120">The list of feed orientations that are supported by the printer.</span></span>|
|<span data-ttu-id="67e17-121">isPageRangeSupported</span><span class="sxs-lookup"><span data-stu-id="67e17-121">isPageRangeSupported</span></span>|<span data-ttu-id="67e17-122">Логический</span><span class="sxs-lookup"><span data-stu-id="67e17-122">Boolean</span></span>|<span data-ttu-id="67e17-123">True, если принтер поддерживает печать по диапазонам страниц; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="67e17-123">True if the printer supports printing by page ranges; false otherwise.</span></span>|
|<span data-ttu-id="67e17-124">качества</span><span class="sxs-lookup"><span data-stu-id="67e17-124">qualities</span></span>|<span data-ttu-id="67e17-125">[коллекция printQuality](enums.md#printquality-values)</span><span class="sxs-lookup"><span data-stu-id="67e17-125">[printQuality](enums.md#printquality-values) collection</span></span>|<span data-ttu-id="67e17-126">Свойства печати, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-126">The print qualities supported by the printer.</span></span>|
|<span data-ttu-id="67e17-127">dpis</span><span class="sxs-lookup"><span data-stu-id="67e17-127">dpis</span></span>|<span data-ttu-id="67e17-128">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="67e17-128">Int32 collection</span></span>|<span data-ttu-id="67e17-129">Список разрешений печати в DPI, поддерживаемых принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-129">The list of print resolutions in DPI that are supported by the printer.</span></span>|
|<span data-ttu-id="67e17-130">duplexModes</span><span class="sxs-lookup"><span data-stu-id="67e17-130">duplexModes</span></span>|<span data-ttu-id="67e17-131">[коллекция printDuplexMode](enums.md#printduplexmode-values)</span><span class="sxs-lookup"><span data-stu-id="67e17-131">[printDuplexMode](enums.md#printduplexmode-values) collection</span></span>|<span data-ttu-id="67e17-132">Список режимов дуплекса, поддерживаемых принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-132">The list of duplex modes that are supported by the printer.</span></span> <span data-ttu-id="67e17-133">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="67e17-133">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="67e17-134">queueBufferSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="67e17-134">queueBufferSizeInBytes</span></span>|<span data-ttu-id="67e17-135">Int32</span><span class="sxs-lookup"><span data-stu-id="67e17-135">Int32</span></span>|<span data-ttu-id="67e17-136">Максимальный размер очереди задания печати, который может храниться на принтере.</span><span class="sxs-lookup"><span data-stu-id="67e17-136">The maximum print job queue size that can be stored by the printer.</span></span>|
|<span data-ttu-id="67e17-137">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="67e17-137">copiesPerJob</span></span>|[<span data-ttu-id="67e17-138">integerRange</span><span class="sxs-lookup"><span data-stu-id="67e17-138">integerRange</span></span>](integerrange.md)|<span data-ttu-id="67e17-139">Диапазон копий на одну работу, поддерживаемую принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-139">The range of copies per job supported by the printer.</span></span>|
|<span data-ttu-id="67e17-140">finishings</span><span class="sxs-lookup"><span data-stu-id="67e17-140">finishings</span></span>|<span data-ttu-id="67e17-141">[коллекция printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="67e17-141">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="67e17-142">Отделочные процессы, поддерживаемые принтером для печатного документа.</span><span class="sxs-lookup"><span data-stu-id="67e17-142">Finishing processes the printer supports for a printed document.</span></span>|
|<span data-ttu-id="67e17-143">mediaColors</span><span class="sxs-lookup"><span data-stu-id="67e17-143">mediaColors</span></span>|<span data-ttu-id="67e17-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67e17-144">String collection</span></span>|<span data-ttu-id="67e17-145">Средства массовой информации (например, бумажные) цвета, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-145">The media (i.e., paper) colors supported by the printer.</span></span>|
|<span data-ttu-id="67e17-146">mediaTypes</span><span class="sxs-lookup"><span data-stu-id="67e17-146">mediaTypes</span></span>|<span data-ttu-id="67e17-147">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67e17-147">String collection</span></span>|<span data-ttu-id="67e17-148">Типы мультимедиа, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-148">The media types supported by the printer.</span></span> <span data-ttu-id="67e17-149">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="67e17-149">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="67e17-150">mediaSizes</span><span class="sxs-lookup"><span data-stu-id="67e17-150">mediaSizes</span></span>|<span data-ttu-id="67e17-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67e17-151">String collection</span></span>|<span data-ttu-id="67e17-152">Размеры мультимедиа, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-152">The media sizes supported by the printer.</span></span> <span data-ttu-id="67e17-153">Поддерживает стандартные имена размеров для средств массовой информации ISO и ANSI, а также любые настраиваемые размеры, поддерживаемые связанным принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-153">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>|
|<span data-ttu-id="67e17-154">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="67e17-154">pagesPerSheet</span></span>|<span data-ttu-id="67e17-155">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="67e17-155">Int32 collection</span></span>|<span data-ttu-id="67e17-156">Поддерживаемое количество страниц ввода, которые необходимо навязать одному впечатлению.</span><span class="sxs-lookup"><span data-stu-id="67e17-156">Supported number of Input Pages to impose upon a single Impression.</span></span>|
|<span data-ttu-id="67e17-157">ориентации</span><span class="sxs-lookup"><span data-stu-id="67e17-157">orientations</span></span>|<span data-ttu-id="67e17-158">[коллекция printOrientation](enums.md#printorientation-values)</span><span class="sxs-lookup"><span data-stu-id="67e17-158">[printOrientation](enums.md#printorientation-values) collection</span></span>|<span data-ttu-id="67e17-159">Ориентации печати, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-159">The print orientations supported by the printer.</span></span> <span data-ttu-id="67e17-160">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="67e17-160">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="67e17-161">inputBins</span><span class="sxs-lookup"><span data-stu-id="67e17-161">inputBins</span></span>|<span data-ttu-id="67e17-162">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67e17-162">String collection</span></span>|<span data-ttu-id="67e17-163">Поддерживаемые ячейки ввода для принтера.</span><span class="sxs-lookup"><span data-stu-id="67e17-163">Supported input bins for the printer.</span></span>|
|<span data-ttu-id="67e17-164">outputBins</span><span class="sxs-lookup"><span data-stu-id="67e17-164">outputBins</span></span>|<span data-ttu-id="67e17-165">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67e17-165">String collection</span></span>|<span data-ttu-id="67e17-166">Поддерживаемые ячейки вывода принтера (лотки).</span><span class="sxs-lookup"><span data-stu-id="67e17-166">The printer's supported output bins (trays).</span></span>|
|<span data-ttu-id="67e17-167">supportsFitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="67e17-167">supportsFitPdfToPage</span></span>|<span data-ttu-id="67e17-168">Логический</span><span class="sxs-lookup"><span data-stu-id="67e17-168">Boolean</span></span>|<span data-ttu-id="67e17-169">True, если принтер поддерживает масштабирование страниц PDF в соответствие с размером печатных мультимедиа; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="67e17-169">True if the printer supports scaling PDF pages to match the print media size; false otherwise.</span></span>|
|<span data-ttu-id="67e17-170">multipageLayouts</span><span class="sxs-lookup"><span data-stu-id="67e17-170">multipageLayouts</span></span>|<span data-ttu-id="67e17-171">[коллекция printMultipageLayout](enums.md#printmultipagelayout-values)</span><span class="sxs-lookup"><span data-stu-id="67e17-171">[printMultipageLayout](enums.md#printmultipagelayout-values) collection</span></span>|<span data-ttu-id="67e17-172">Направления презентации, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-172">The presentation directions supported by the printer.</span></span> <span data-ttu-id="67e17-173">Поддерживаемые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="67e17-173">Supported values are described in the following table.</span></span>|
|<span data-ttu-id="67e17-174">colorModes</span><span class="sxs-lookup"><span data-stu-id="67e17-174">colorModes</span></span>|<span data-ttu-id="67e17-175">[коллекция printColorMode](enums.md#printcolormode-values)</span><span class="sxs-lookup"><span data-stu-id="67e17-175">[printColorMode](enums.md#printcolormode-values) collection</span></span>|<span data-ttu-id="67e17-176">Цветовые режимы, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="67e17-176">The color modes supported by the printer.</span></span> <span data-ttu-id="67e17-177">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="67e17-177">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="67e17-178">topMargins</span><span class="sxs-lookup"><span data-stu-id="67e17-178">topMargins</span></span>|<span data-ttu-id="67e17-179">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="67e17-179">Int32 collection</span></span>|<span data-ttu-id="67e17-180">Список поддерживаемых верхних полей (в микронах) для принтера.</span><span class="sxs-lookup"><span data-stu-id="67e17-180">A list of supported top margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="67e17-181">bottomMargins</span><span class="sxs-lookup"><span data-stu-id="67e17-181">bottomMargins</span></span>|<span data-ttu-id="67e17-182">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="67e17-182">Int32 collection</span></span>|<span data-ttu-id="67e17-183">Список поддерживаемых нижних полей (в микронах) для принтера.</span><span class="sxs-lookup"><span data-stu-id="67e17-183">A list of supported bottom margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="67e17-184">rightMargins</span><span class="sxs-lookup"><span data-stu-id="67e17-184">rightMargins</span></span>|<span data-ttu-id="67e17-185">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="67e17-185">Int32 collection</span></span>|<span data-ttu-id="67e17-186">Список поддерживаемых правых полей (в микронах) для принтера.</span><span class="sxs-lookup"><span data-stu-id="67e17-186">A list of supported right margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="67e17-187">leftMargins</span><span class="sxs-lookup"><span data-stu-id="67e17-187">leftMargins</span></span>|<span data-ttu-id="67e17-188">Коллекция Int32</span><span class="sxs-lookup"><span data-stu-id="67e17-188">Int32 collection</span></span>|<span data-ttu-id="67e17-189">Список поддерживаемых левых полей (в микронах) для принтера.</span><span class="sxs-lookup"><span data-stu-id="67e17-189">A list of supported left margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="67e17-190">collation</span><span class="sxs-lookup"><span data-stu-id="67e17-190">collation</span></span>|<span data-ttu-id="67e17-191">Логический</span><span class="sxs-lookup"><span data-stu-id="67e17-191">Boolean</span></span>|<span data-ttu-id="67e17-192">True, если принтер поддерживает копирование при печати muliple копий многошагового документа; false в противном случае.</span><span class="sxs-lookup"><span data-stu-id="67e17-192">True if the printer supports collating when printing muliple copies of a multi-page document; false otherwise.</span></span>|
|<span data-ttu-id="67e17-193">scalings</span><span class="sxs-lookup"><span data-stu-id="67e17-193">scalings</span></span>|<span data-ttu-id="67e17-194">[коллекция printScaling](enums.md#printscaling-values)</span><span class="sxs-lookup"><span data-stu-id="67e17-194">[printScaling](enums.md#printscaling-values) collection</span></span>|<span data-ttu-id="67e17-195">Поддерживаемые масштабирования печати.</span><span class="sxs-lookup"><span data-stu-id="67e17-195">Supported print scalings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67e17-196">Отношения</span><span class="sxs-lookup"><span data-stu-id="67e17-196">Relationships</span></span>
<span data-ttu-id="67e17-197">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="67e17-197">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67e17-198">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="67e17-198">JSON representation</span></span>
<span data-ttu-id="67e17-199">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67e17-199">The following is a JSON representation of the resource.</span></span>
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

