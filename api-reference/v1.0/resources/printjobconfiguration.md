---
title: тип ресурса printJobConfiguration
description: Группа параметров, которые принтер должен использовать для печати задания.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1e12541bd4426dca1e0d7b48b0e3bcbd9e2bb7ea
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518065"
---
# <a name="printjobconfiguration-resource-type"></a><span data-ttu-id="7352f-103">тип ресурса printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="7352f-103">printJobConfiguration resource type</span></span>

<span data-ttu-id="7352f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7352f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7352f-105">Группа параметров, которые принтер должен использовать для печати задания.</span><span class="sxs-lookup"><span data-stu-id="7352f-105">A group of settings that a printer should use to print a job.</span></span>

## <a name="properties"></a><span data-ttu-id="7352f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7352f-106">Properties</span></span>
|<span data-ttu-id="7352f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7352f-107">Property</span></span>|<span data-ttu-id="7352f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7352f-108">Type</span></span>|<span data-ttu-id="7352f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7352f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7352f-110">pageRanges</span><span class="sxs-lookup"><span data-stu-id="7352f-110">pageRanges</span></span>|<span data-ttu-id="7352f-111">[коллекция integerRange](integerrange.md)</span><span class="sxs-lookup"><span data-stu-id="7352f-111">[integerRange](integerrange.md) collection</span></span>|<span data-ttu-id="7352f-112">Страница колеблется для печати.</span><span class="sxs-lookup"><span data-stu-id="7352f-112">The page ranges to print.</span></span> <span data-ttu-id="7352f-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7352f-113">Read-only.</span></span>|
|<span data-ttu-id="7352f-114">качество</span><span class="sxs-lookup"><span data-stu-id="7352f-114">quality</span></span>|[<span data-ttu-id="7352f-115">printQuality</span><span class="sxs-lookup"><span data-stu-id="7352f-115">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="7352f-116">Качество печати, используемой при печати задания.</span><span class="sxs-lookup"><span data-stu-id="7352f-116">The print quality to use when printing the job.</span></span> <span data-ttu-id="7352f-117">Допустимые значения описаны в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="7352f-117">Valid values are described in the table below.</span></span> <span data-ttu-id="7352f-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7352f-118">Read-only.</span></span>|
|<span data-ttu-id="7352f-119">dpi</span><span class="sxs-lookup"><span data-stu-id="7352f-119">dpi</span></span>|<span data-ttu-id="7352f-120">Int32</span><span class="sxs-lookup"><span data-stu-id="7352f-120">Int32</span></span>|<span data-ttu-id="7352f-121">Разрешение, используемого при печати задания, выраженного точками на дюйм (DPI).</span><span class="sxs-lookup"><span data-stu-id="7352f-121">The resolution to use when printing the job, expressed in dots per inch (DPI).</span></span> <span data-ttu-id="7352f-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7352f-122">Read-only.</span></span>|
|<span data-ttu-id="7352f-123">feedOrientation</span><span class="sxs-lookup"><span data-stu-id="7352f-123">feedOrientation</span></span>|<span data-ttu-id="7352f-124">printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="7352f-124">printerFeedOrientation</span></span>|<span data-ttu-id="7352f-125">Ориентация, используемая при подаче носителю в принтер.</span><span class="sxs-lookup"><span data-stu-id="7352f-125">The orientation to use when feeding media into the printer.</span></span> <span data-ttu-id="7352f-126">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7352f-126">Valid values are described in the following table.</span></span> <span data-ttu-id="7352f-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7352f-127">Read-only.</span></span>|
|<span data-ttu-id="7352f-128">orientation</span><span class="sxs-lookup"><span data-stu-id="7352f-128">orientation</span></span>|[<span data-ttu-id="7352f-129">printOrientation</span><span class="sxs-lookup"><span data-stu-id="7352f-129">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="7352f-130">Параметр ориентации, который принтер должен использовать при печати задания.</span><span class="sxs-lookup"><span data-stu-id="7352f-130">The orientation setting the printer should use when printing the job.</span></span> <span data-ttu-id="7352f-131">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7352f-131">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="7352f-132">duplexMode</span><span class="sxs-lookup"><span data-stu-id="7352f-132">duplexMode</span></span>|[<span data-ttu-id="7352f-133">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="7352f-133">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="7352f-134">Режим дуплекса, который принтер должен использовать при печати задания.</span><span class="sxs-lookup"><span data-stu-id="7352f-134">The duplex mode the printer should use when printing the job.</span></span> <span data-ttu-id="7352f-135">Допустимые значения описаны в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="7352f-135">Valid values are described in the table below.</span></span> <span data-ttu-id="7352f-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7352f-136">Read-only.</span></span>|
|<span data-ttu-id="7352f-137">копии</span><span class="sxs-lookup"><span data-stu-id="7352f-137">copies</span></span>|<span data-ttu-id="7352f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7352f-138">Int32</span></span>|<span data-ttu-id="7352f-139">Количество копий, которые должны быть напечатаны.</span><span class="sxs-lookup"><span data-stu-id="7352f-139">The number of copies that should be printed.</span></span> <span data-ttu-id="7352f-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7352f-140">Read-only.</span></span>|
|<span data-ttu-id="7352f-141">colorMode</span><span class="sxs-lookup"><span data-stu-id="7352f-141">colorMode</span></span>|[<span data-ttu-id="7352f-142">printColorMode</span><span class="sxs-lookup"><span data-stu-id="7352f-142">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="7352f-143">Цветовой режим, который принтер должен использовать для печати задания.</span><span class="sxs-lookup"><span data-stu-id="7352f-143">The color mode the printer should use to print the job.</span></span> <span data-ttu-id="7352f-144">Допустимые значения описаны в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="7352f-144">Valid values are described in the table below.</span></span> <span data-ttu-id="7352f-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7352f-145">Read-only.</span></span>|
|<span data-ttu-id="7352f-146">inputBin</span><span class="sxs-lookup"><span data-stu-id="7352f-146">inputBin</span></span>|<span data-ttu-id="7352f-147">Строка</span><span class="sxs-lookup"><span data-stu-id="7352f-147">String</span></span>|<span data-ttu-id="7352f-148">Ячейка ввода (лоток), используемая при печати.</span><span class="sxs-lookup"><span data-stu-id="7352f-148">The input bin (tray) to use when printing.</span></span> <span data-ttu-id="7352f-149">Сведения о возможностях [принтера см.](printercapabilities.md) в списке поддерживаемых корзин ввода.</span><span class="sxs-lookup"><span data-stu-id="7352f-149">See the printer's [capabilities](printercapabilities.md) for a list of supported input bins.</span></span>|
|<span data-ttu-id="7352f-150">outputBin</span><span class="sxs-lookup"><span data-stu-id="7352f-150">outputBin</span></span>|<span data-ttu-id="7352f-151">Строка</span><span class="sxs-lookup"><span data-stu-id="7352f-151">String</span></span>|<span data-ttu-id="7352f-152">Ячейка вывода, в который можно разместить завершенные отпечатки.</span><span class="sxs-lookup"><span data-stu-id="7352f-152">The output bin to place completed prints into.</span></span> <span data-ttu-id="7352f-153">См. возможности [принтера для](printercapabilities.md) списка поддерживаемых бункеров выходных данных.</span><span class="sxs-lookup"><span data-stu-id="7352f-153">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="7352f-154">mediaSize</span><span class="sxs-lookup"><span data-stu-id="7352f-154">mediaSize</span></span>|<span data-ttu-id="7352f-155">Строка</span><span class="sxs-lookup"><span data-stu-id="7352f-155">String</span></span>|<span data-ttu-id="7352f-156">Размер мультимедиа, который используется при печати.</span><span class="sxs-lookup"><span data-stu-id="7352f-156">The media sizeto use when printing.</span></span> <span data-ttu-id="7352f-157">Поддерживает стандартные имена размеров для средств массовой информации ISO и ANSI, а также любые настраиваемые размеры, поддерживаемые связанным принтером.</span><span class="sxs-lookup"><span data-stu-id="7352f-157">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>|
|<span data-ttu-id="7352f-158">margin</span><span class="sxs-lookup"><span data-stu-id="7352f-158">margin</span></span>|[<span data-ttu-id="7352f-159">printMargin</span><span class="sxs-lookup"><span data-stu-id="7352f-159">printMargin</span></span>](printmargin.md)|<span data-ttu-id="7352f-160">Параметры поля, которые необходимо использовать при печати.</span><span class="sxs-lookup"><span data-stu-id="7352f-160">The margin settings to use when printing.</span></span>|
|<span data-ttu-id="7352f-161">MediaType</span><span class="sxs-lookup"><span data-stu-id="7352f-161">mediaType</span></span>|<span data-ttu-id="7352f-162">Строка</span><span class="sxs-lookup"><span data-stu-id="7352f-162">String</span></span>|<span data-ttu-id="7352f-163">Тип мультимедиа по умолчанию (например, бумага) для печати документа.</span><span class="sxs-lookup"><span data-stu-id="7352f-163">The default media (such as paper) type to print the document on.</span></span> <span data-ttu-id="7352f-164">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7352f-164">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="7352f-165">finishings</span><span class="sxs-lookup"><span data-stu-id="7352f-165">finishings</span></span>|<span data-ttu-id="7352f-166">[коллекция printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="7352f-166">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="7352f-167">Отделочные процессы, которые необходимо использовать при печати.</span><span class="sxs-lookup"><span data-stu-id="7352f-167">Finishing processes to use when printing.</span></span>|
|<span data-ttu-id="7352f-168">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="7352f-168">pagesPerSheet</span></span>|<span data-ttu-id="7352f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="7352f-169">Int32</span></span>|<span data-ttu-id="7352f-170">Количество страниц документов для печати на каждом листе.</span><span class="sxs-lookup"><span data-stu-id="7352f-170">The number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="7352f-171">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="7352f-171">multipageLayout</span></span>|[<span data-ttu-id="7352f-172">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="7352f-172">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="7352f-173">Направление для раскладывки страниц при печати нескольких страниц на один лист.</span><span class="sxs-lookup"><span data-stu-id="7352f-173">The direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="7352f-174">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7352f-174">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="7352f-175">collate</span><span class="sxs-lookup"><span data-stu-id="7352f-175">collate</span></span>|<span data-ttu-id="7352f-176">Логический</span><span class="sxs-lookup"><span data-stu-id="7352f-176">Boolean</span></span>|<span data-ttu-id="7352f-177">Должен ли принтер совмессировать страницы, печатая несколько копий много страниц документа.</span><span class="sxs-lookup"><span data-stu-id="7352f-177">Whether the printer should collate pages wehen printing multiple copies of a multi-page document.</span></span>|
|<span data-ttu-id="7352f-178">scaling</span><span class="sxs-lookup"><span data-stu-id="7352f-178">scaling</span></span>|[<span data-ttu-id="7352f-179">printScaling</span><span class="sxs-lookup"><span data-stu-id="7352f-179">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="7352f-180">Указывает, как принтер должен масштабировать данные документа, чтобы соответствовать запрашиваемой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="7352f-180">Specifies how the printer should scale the document data to fit the requested media.</span></span> <span data-ttu-id="7352f-181">Допустимые значения описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7352f-181">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7352f-182">Отношения</span><span class="sxs-lookup"><span data-stu-id="7352f-182">Relationships</span></span>
<span data-ttu-id="7352f-183">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7352f-183">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7352f-184">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7352f-184">JSON representation</span></span>
<span data-ttu-id="7352f-185">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7352f-185">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobConfiguration",
  "pageRanges": [
    {
      "@odata.type": "microsoft.graph.integerRange"
    }
  ],
  "quality": "String",
  "dpi": "Integer",
  "feedOrientation": "String",
  "orientation": "String",
  "duplexMode": "String",
  "copies": "Integer",
  "colorMode": "String",
  "inputBin": "String",
  "outputBin": "String",
  "mediaSize": "String",
  "margin": {
    "@odata.type": "microsoft.graph.printMargin"
  },
  "mediaType": "String",
  "finishings": [
    "String"
  ],
  "pagesPerSheet": "Integer",
  "multipageLayout": "String",
  "collate": "Boolean",
  "scaling": "String",
  "fitPdfToPage": "Boolean"
}
```

