---
title: Тип ресурса Принтердокументконфигуратион
description: Группа параметров, которые принтер должен использовать для печати документа.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ff1da92894f8854bcdee2ce24d7a9d5cef6288e7
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896023"
---
# <a name="printerdocumentconfiguration-resource-type"></a><span data-ttu-id="9acfe-103">Тип ресурса Принтердокументконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9acfe-103">printerDocumentConfiguration resource type</span></span>

<span data-ttu-id="9acfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9acfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9acfe-105">Группа параметров, которые принтер должен использовать для печати документа.</span><span class="sxs-lookup"><span data-stu-id="9acfe-105">A group of settings that a printer should use to print a document.</span></span>

## <a name="properties"></a><span data-ttu-id="9acfe-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9acfe-106">Properties</span></span>
| <span data-ttu-id="9acfe-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9acfe-107">Property</span></span>     | <span data-ttu-id="9acfe-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9acfe-108">Type</span></span>        | <span data-ttu-id="9acfe-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9acfe-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9acfe-110">пажеранжес</span><span class="sxs-lookup"><span data-stu-id="9acfe-110">pageRanges</span></span>|<span data-ttu-id="9acfe-111">Коллекция [принтпажеранже](printpagerange.md)</span><span class="sxs-lookup"><span data-stu-id="9acfe-111">[printPageRange](printpagerange.md) collection</span></span>|<span data-ttu-id="9acfe-112">Диапазоны страниц для печати.</span><span class="sxs-lookup"><span data-stu-id="9acfe-112">The page ranges to print.</span></span> <span data-ttu-id="9acfe-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9acfe-113">Read-only.</span></span>|
|<span data-ttu-id="9acfe-114">принткуалити</span><span class="sxs-lookup"><span data-stu-id="9acfe-114">printQuality</span></span>|<span data-ttu-id="9acfe-115">принткуалити</span><span class="sxs-lookup"><span data-stu-id="9acfe-115">printQuality</span></span>|<span data-ttu-id="9acfe-116">Качество печати, используемое при печати задания.</span><span class="sxs-lookup"><span data-stu-id="9acfe-116">The print quality to use when printing the job.</span></span> <span data-ttu-id="9acfe-117">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="9acfe-117">Valid values are described in the table below.</span></span> <span data-ttu-id="9acfe-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9acfe-118">Read-only.</span></span>|
|<span data-ttu-id="9acfe-119">принтресолутиониндпи</span><span class="sxs-lookup"><span data-stu-id="9acfe-119">printResolutionInDpi</span></span>|<span data-ttu-id="9acfe-120">Int32</span><span class="sxs-lookup"><span data-stu-id="9acfe-120">Int32</span></span>|<span data-ttu-id="9acfe-121">Решение, используемое при печати задания, выраженное в точках на дюйм (DPI).</span><span class="sxs-lookup"><span data-stu-id="9acfe-121">The resolution to use when printing the job, expressed in dots per inch (DPI).</span></span> <span data-ttu-id="9acfe-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9acfe-122">Read-only.</span></span>|
|<span data-ttu-id="9acfe-123">фиддиректион</span><span class="sxs-lookup"><span data-stu-id="9acfe-123">feedDirection</span></span>|<span data-ttu-id="9acfe-124">принтерфиддиректион</span><span class="sxs-lookup"><span data-stu-id="9acfe-124">printerFeedDirection</span></span>|<span data-ttu-id="9acfe-125">Направление, используемое при выдачах мультимедиа на принтер.</span><span class="sxs-lookup"><span data-stu-id="9acfe-125">The direction to use when feeding media into the printer.</span></span> <span data-ttu-id="9acfe-126">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="9acfe-126">Valid values are described in the following table.</span></span> <span data-ttu-id="9acfe-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9acfe-127">Read-only.</span></span>|
|<span data-ttu-id="9acfe-128">orientation</span><span class="sxs-lookup"><span data-stu-id="9acfe-128">orientation</span></span>|<span data-ttu-id="9acfe-129">принториентатион</span><span class="sxs-lookup"><span data-stu-id="9acfe-129">printOrientation</span></span>|<span data-ttu-id="9acfe-130">Параметр Orientation, который должен использоваться принтером при печати задания.</span><span class="sxs-lookup"><span data-stu-id="9acfe-130">The orientation setting the printer should use when printing the job.</span></span> <span data-ttu-id="9acfe-131">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="9acfe-131">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="9acfe-132">дуплексконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9acfe-132">duplexConfiguration</span></span>|<span data-ttu-id="9acfe-133">принтдуплексконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9acfe-133">printDuplexConfiguration</span></span>|<span data-ttu-id="9acfe-134">Дуплексная конфигурация, которая должна использоваться принтером при печати задания.</span><span class="sxs-lookup"><span data-stu-id="9acfe-134">The duplex configuration the printer should use when printing the job.</span></span> <span data-ttu-id="9acfe-135">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="9acfe-135">Valid values are described in the table below.</span></span> <span data-ttu-id="9acfe-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9acfe-136">Read-only.</span></span>|
|<span data-ttu-id="9acfe-137">скопирует</span><span class="sxs-lookup"><span data-stu-id="9acfe-137">copies</span></span>|<span data-ttu-id="9acfe-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9acfe-138">Int32</span></span>|<span data-ttu-id="9acfe-139">Количество копий, которое необходимо напечатать.</span><span class="sxs-lookup"><span data-stu-id="9acfe-139">The number of copies that should be printed.</span></span> <span data-ttu-id="9acfe-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9acfe-140">Read-only.</span></span>|
|<span data-ttu-id="9acfe-141">колорконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9acfe-141">colorConfiguration</span></span>|<span data-ttu-id="9acfe-142">принтколорконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9acfe-142">printColorConfiguration</span></span>|<span data-ttu-id="9acfe-143">Цветовая конфигурация, которую должен использовать принтер для печати задания.</span><span class="sxs-lookup"><span data-stu-id="9acfe-143">The color configuration the printer should use to print the job.</span></span> <span data-ttu-id="9acfe-144">Допустимые значения описаны в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="9acfe-144">Valid values are described in the table below.</span></span> <span data-ttu-id="9acfe-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9acfe-145">Read-only.</span></span>|

### <a name="printduplexconfiguration-values"></a><span data-ttu-id="9acfe-146">значения Принтдуплексконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9acfe-146">printDuplexConfiguration values</span></span>

|<span data-ttu-id="9acfe-147">Элемент</span><span class="sxs-lookup"><span data-stu-id="9acfe-147">Member</span></span>|<span data-ttu-id="9acfe-148">Значение</span><span class="sxs-lookup"><span data-stu-id="9acfe-148">Value</span></span>|<span data-ttu-id="9acfe-149">Описание</span><span class="sxs-lookup"><span data-stu-id="9acfe-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9acfe-150">твосидедлонжедже</span><span class="sxs-lookup"><span data-stu-id="9acfe-150">twoSidedLongEdge</span></span>|<span data-ttu-id="9acfe-151">нуль</span><span class="sxs-lookup"><span data-stu-id="9acfe-151">0</span></span>|<span data-ttu-id="9acfe-152">Принтер будет печататься на двух сторонах и будет переворачивать документы вдоль длинного края.</span><span class="sxs-lookup"><span data-stu-id="9acfe-152">The printer will print double-sided, and will flip documents along the long edge.</span></span>|
|<span data-ttu-id="9acfe-153">твосидедшортедже</span><span class="sxs-lookup"><span data-stu-id="9acfe-153">twoSidedShortEdge</span></span>|<span data-ttu-id="9acfe-154">1,1</span><span class="sxs-lookup"><span data-stu-id="9acfe-154">1</span></span>|<span data-ttu-id="9acfe-155">Принтер будет печататься на двух сторонах и будет переражать документы вдоль короткого края.</span><span class="sxs-lookup"><span data-stu-id="9acfe-155">The printer will print double-sided, and will flip documents along the short edge.</span></span>|
|<span data-ttu-id="9acfe-156">онесидед</span><span class="sxs-lookup"><span data-stu-id="9acfe-156">oneSided</span></span>|<span data-ttu-id="9acfe-157">2</span><span class="sxs-lookup"><span data-stu-id="9acfe-157">2</span></span>|<span data-ttu-id="9acfe-158">На принтере будет напечатана только одна сторона.</span><span class="sxs-lookup"><span data-stu-id="9acfe-158">The printer will print single-sided.</span></span>|

### <a name="printquality-values"></a><span data-ttu-id="9acfe-159">значения Принткуалити</span><span class="sxs-lookup"><span data-stu-id="9acfe-159">printQuality values</span></span>

|<span data-ttu-id="9acfe-160">Member</span><span class="sxs-lookup"><span data-stu-id="9acfe-160">Member</span></span>|<span data-ttu-id="9acfe-161">Описание</span><span class="sxs-lookup"><span data-stu-id="9acfe-161">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9acfe-162">потребление</span><span class="sxs-lookup"><span data-stu-id="9acfe-162">low</span></span>|<span data-ttu-id="9acfe-163">Принтер выполнит печать задания, используя низкую (обычно называемую "черновой") качеством.</span><span class="sxs-lookup"><span data-stu-id="9acfe-163">The printer will print the job using low (commonly known as "draft") quality.</span></span>|
|<span data-ttu-id="9acfe-164">medium</span><span class="sxs-lookup"><span data-stu-id="9acfe-164">medium</span></span>|<span data-ttu-id="9acfe-165">Принтер выполнит печать задания, используя медим (обычно известное как "нормальное").</span><span class="sxs-lookup"><span data-stu-id="9acfe-165">The printer will print the job using medim (commonly known as "normal") quality.</span></span>|
|<span data-ttu-id="9acfe-166">высокоуровневых</span><span class="sxs-lookup"><span data-stu-id="9acfe-166">high</span></span>|<span data-ttu-id="9acfe-167">Принтер выполнит печать задания, используя высокое (обычное, известное как "наилучшее" или "точное") качество.</span><span class="sxs-lookup"><span data-stu-id="9acfe-167">The printer will print the job using high (commonly known as "best" or "fine") quality.</span></span>|

## <a name="printerfeeddirection-values"></a><span data-ttu-id="9acfe-168">значения Принтерфиддиректион</span><span class="sxs-lookup"><span data-stu-id="9acfe-168">printerFeedDirection values</span></span>

|<span data-ttu-id="9acfe-169">Member</span><span class="sxs-lookup"><span data-stu-id="9acfe-169">Member</span></span>|<span data-ttu-id="9acfe-170">Описание</span><span class="sxs-lookup"><span data-stu-id="9acfe-170">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9acfe-171">лонжеджефирст</span><span class="sxs-lookup"><span data-stu-id="9acfe-171">longEdgeFirst</span></span>|<span data-ttu-id="9acfe-172">Принтер будет использовать листы из активного лотка на "альбомной" ориентации, с длинным краем листа.</span><span class="sxs-lookup"><span data-stu-id="9acfe-172">The printer will consume sheets from the active tray in "landscape" orientation, with the long edge of the sheet first.</span></span>|
|<span data-ttu-id="9acfe-173">шортеджефирст</span><span class="sxs-lookup"><span data-stu-id="9acfe-173">shortEdgeFirst</span></span>|<span data-ttu-id="9acfe-174">Принтер будет использовать листы из активного лотка на странице "Книжная" (ориентация), при этом сначала используется короткий край листа.</span><span class="sxs-lookup"><span data-stu-id="9acfe-174">The printer will consume sheets from the active tray in "portrait" orientation, with the short edge of the sheet first.</span></span>|

## <a name="printorientation-values"></a><span data-ttu-id="9acfe-175">значения Принториентатион</span><span class="sxs-lookup"><span data-stu-id="9acfe-175">printOrientation values</span></span>

|<span data-ttu-id="9acfe-176">Элемент</span><span class="sxs-lookup"><span data-stu-id="9acfe-176">Member</span></span>|<span data-ttu-id="9acfe-177">Значение</span><span class="sxs-lookup"><span data-stu-id="9acfe-177">Value</span></span>|<span data-ttu-id="9acfe-178">Описание</span><span class="sxs-lookup"><span data-stu-id="9acfe-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9acfe-179">ориентацию</span><span class="sxs-lookup"><span data-stu-id="9acfe-179">portrait</span></span>|<span data-ttu-id="9acfe-180">4</span><span class="sxs-lookup"><span data-stu-id="9acfe-180">3</span></span>|<span data-ttu-id="9acfe-181">Принтер будет печатать впечатления в "книжной" ориентации.</span><span class="sxs-lookup"><span data-stu-id="9acfe-181">The printer will print impressions in the "portrait" orientation.</span></span>|
|<span data-ttu-id="9acfe-182">вдоль</span><span class="sxs-lookup"><span data-stu-id="9acfe-182">landscape</span></span>|<span data-ttu-id="9acfe-183">4 </span><span class="sxs-lookup"><span data-stu-id="9acfe-183">4</span></span>|<span data-ttu-id="9acfe-184">Принтер будет печатать впечатления на "альбомной" ориентации.</span><span class="sxs-lookup"><span data-stu-id="9acfe-184">The printer will print impressions in the "landscape" orientation.</span></span>|
|<span data-ttu-id="9acfe-185">реверселандскапе</span><span class="sxs-lookup"><span data-stu-id="9acfe-185">reverseLandscape</span></span>|<span data-ttu-id="9acfe-186">5 </span><span class="sxs-lookup"><span data-stu-id="9acfe-186">5</span></span>|<span data-ttu-id="9acfe-187">Принтер будет печатать впечатления на ориентации "Обратная ориентация".</span><span class="sxs-lookup"><span data-stu-id="9acfe-187">The printer will print impressions in the "reverse landscape" orientation.</span></span>|
|<span data-ttu-id="9acfe-188">реверсепортраит</span><span class="sxs-lookup"><span data-stu-id="9acfe-188">reversePortrait</span></span>|<span data-ttu-id="9acfe-189">6 </span><span class="sxs-lookup"><span data-stu-id="9acfe-189">6</span></span>|<span data-ttu-id="9acfe-190">Принтер будет печатать впечатления на ориентации "Обратная книжная".</span><span class="sxs-lookup"><span data-stu-id="9acfe-190">The printer will print impressions in the "reverse portrait" orientation.</span></span>|

### <a name="printcolorconfiguration-values"></a><span data-ttu-id="9acfe-191">значения Принтколорконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9acfe-191">printColorConfiguration values</span></span>

|<span data-ttu-id="9acfe-192">Элемент</span><span class="sxs-lookup"><span data-stu-id="9acfe-192">Member</span></span>|<span data-ttu-id="9acfe-193">Значение</span><span class="sxs-lookup"><span data-stu-id="9acfe-193">Value</span></span>|<span data-ttu-id="9acfe-194">Описание</span><span class="sxs-lookup"><span data-stu-id="9acfe-194">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9acfe-195">блаккандвхите</span><span class="sxs-lookup"><span data-stu-id="9acfe-195">blackAndWhite</span></span>|<span data-ttu-id="9acfe-196">нуль</span><span class="sxs-lookup"><span data-stu-id="9acfe-196">0</span></span>|<span data-ttu-id="9acfe-197">Черно-белое (используйте только черные материалы с маркерами).</span><span class="sxs-lookup"><span data-stu-id="9acfe-197">Black and white (use black marker material only.)</span></span>|
|<span data-ttu-id="9acfe-198">черн</span><span class="sxs-lookup"><span data-stu-id="9acfe-198">grayscale</span></span>|<span data-ttu-id="9acfe-199">1,1</span><span class="sxs-lookup"><span data-stu-id="9acfe-199">1</span></span>|<span data-ttu-id="9acfe-200">Оттенки серого (могут использоваться некоторые материалы цветового маркера).</span><span class="sxs-lookup"><span data-stu-id="9acfe-200">Grayscale (may use some color marker material.)</span></span>|
|<span data-ttu-id="9acfe-201">color</span><span class="sxs-lookup"><span data-stu-id="9acfe-201">color</span></span>|<span data-ttu-id="9acfe-202">2</span><span class="sxs-lookup"><span data-stu-id="9acfe-202">2</span></span>|<span data-ttu-id="9acfe-203">Color (Используйте любую комбинацию материалов маркера, чтобы создать впечатление цвета).</span><span class="sxs-lookup"><span data-stu-id="9acfe-203">Color (use any combination of marker materials to create a color impression).</span></span>|
|<span data-ttu-id="9acfe-204">Авто</span><span class="sxs-lookup"><span data-stu-id="9acfe-204">auto</span></span>|<span data-ttu-id="9acfe-205">4</span><span class="sxs-lookup"><span data-stu-id="9acfe-205">3</span></span>|<span data-ttu-id="9acfe-206">Разрешите принтеру выбрать используемый цветовой режим.</span><span class="sxs-lookup"><span data-stu-id="9acfe-206">Let the printer decide which color mode to use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9acfe-207">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9acfe-207">JSON representation</span></span>

<span data-ttu-id="9acfe-208">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9acfe-208">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerDocumentConfiguration"
}-->

```json
{
  "pageRanges": [{"@odata.type": "microsoft.graph.printPageRange"}],
  "printQuality": "String",
  "printResolutionInDpi": 123456,
  "feedDirection": "String",
  "orientation": "String",
  "duplexConfiguration": "String",
  "copies": 123456,
  "colorConfiguration": "String",
}

```
