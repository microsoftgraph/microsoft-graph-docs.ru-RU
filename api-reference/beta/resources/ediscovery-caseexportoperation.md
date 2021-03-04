---
title: тип ресурса caseExportOperation
description: Представляет процесс экспорта электронных открытий.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c14f4211706879a6897b5f795202a30058d138bf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447578"
---
# <a name="caseexportoperation-resource-type"></a><span data-ttu-id="0fd6b-103">тип ресурса caseExportOperation</span><span class="sxs-lookup"><span data-stu-id="0fd6b-103">caseExportOperation resource type</span></span>

<span data-ttu-id="0fd6b-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0fd6b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fd6b-105">Представляет процесс экспорта электронных открытий.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-105">Represents the process of an eDiscovery export.</span></span> <span data-ttu-id="0fd6b-106">The **caseExportOperation** can only be retrieved from the `Location` header in the response to a [reviewset export.](../api/ediscovery-reviewset-export.md)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-106">The **caseExportOperation** can only be retrieved from the `Location` header in the response to a [reviewset export](../api/ediscovery-reviewset-export.md).</span></span>

<span data-ttu-id="0fd6b-107">Наследует [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0fd6b-107">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0fd6b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0fd6b-108">Methods</span></span>

|<span data-ttu-id="0fd6b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0fd6b-109">Method</span></span>|<span data-ttu-id="0fd6b-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="0fd6b-110">Return type</span></span>|<span data-ttu-id="0fd6b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd6b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fd6b-112">getDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="0fd6b-112">getDownloadUrl</span></span>](../api/ediscovery-caseexportoperation-getdownloadurl.md)|<span data-ttu-id="0fd6b-113">String</span><span class="sxs-lookup"><span data-stu-id="0fd6b-113">String</span></span>| <span data-ttu-id="0fd6b-114">Возвращает URL-адрес для экспорта.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-114">Returns the URL for the export.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fd6b-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fd6b-115">Properties</span></span>

|<span data-ttu-id="0fd6b-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fd6b-116">Property</span></span>|<span data-ttu-id="0fd6b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0fd6b-117">Type</span></span>|<span data-ttu-id="0fd6b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd6b-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fd6b-119">action</span><span class="sxs-lookup"><span data-stu-id="0fd6b-119">action</span></span>|[<span data-ttu-id="0fd6b-120">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="0fd6b-120">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="0fd6b-121">Действие случая для этой сущности всегда будет `contentExport` .</span><span class="sxs-lookup"><span data-stu-id="0fd6b-121">The case action for this entity will always be `contentExport`.</span></span> <span data-ttu-id="0fd6b-122">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0fd6b-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="0fd6b-123">azureBlobContainer</span><span class="sxs-lookup"><span data-stu-id="0fd6b-123">azureBlobContainer</span></span>|<span data-ttu-id="0fd6b-124">String</span><span class="sxs-lookup"><span data-stu-id="0fd6b-124">String</span></span>| <span data-ttu-id="0fd6b-125">Имя расположения хранилища Azure, в котором будет храниться экспорт.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-125">The name of the Azure storage location where the export will be stored.</span></span> <span data-ttu-id="0fd6b-126">Это относится только к экспорту, хранямуся в вашем собственном хранилище Azure.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-126">This only applies to exports stored in your own Azure storage location.</span></span> |
|<span data-ttu-id="0fd6b-127">azureBlobToken</span><span class="sxs-lookup"><span data-stu-id="0fd6b-127">azureBlobToken</span></span>|<span data-ttu-id="0fd6b-128">String</span><span class="sxs-lookup"><span data-stu-id="0fd6b-128">String</span></span>| <span data-ttu-id="0fd6b-129">Маркер SAS для хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-129">The SAS token for the Azure storage location.</span></span>  <span data-ttu-id="0fd6b-130">Это относится только к экспорту, хранямуся в вашем собственном хранилище Azure.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-130">This only applies to exports stored in your own Azure storage location.</span></span> |
|<span data-ttu-id="0fd6b-131">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd6b-131">completedDateTime</span></span>|<span data-ttu-id="0fd6b-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd6b-132">DateTimeOffset</span></span>| <span data-ttu-id="0fd6b-133">Дата и время завершения экспорта.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-133">The date and time the export was completed.</span></span>  <span data-ttu-id="0fd6b-134">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-134">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="0fd6b-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="0fd6b-135">createdBy</span></span>|[<span data-ttu-id="0fd6b-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="0fd6b-136">identitySet</span></span>](../resources/identityset.md)| <span data-ttu-id="0fd6b-137">Пользователь, который инициировал экспортную операцию.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-137">The user who initiated the export operation.</span></span> <span data-ttu-id="0fd6b-138">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-138">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="0fd6b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd6b-139">createdDateTime</span></span>|<span data-ttu-id="0fd6b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd6b-140">DateTimeOffset</span></span>| <span data-ttu-id="0fd6b-141">Дата и время создания экспорта.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-141">The date and time the export was created.</span></span> <span data-ttu-id="0fd6b-142">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="0fd6b-143">description</span><span class="sxs-lookup"><span data-stu-id="0fd6b-143">description</span></span>|<span data-ttu-id="0fd6b-144">String</span><span class="sxs-lookup"><span data-stu-id="0fd6b-144">String</span></span>| <span data-ttu-id="0fd6b-145">Описание, предоставленное для экспорта.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-145">The description provided for the export.</span></span> |
|<span data-ttu-id="0fd6b-146">ExportOptions</span><span class="sxs-lookup"><span data-stu-id="0fd6b-146">exportOptions</span></span>|<span data-ttu-id="0fd6b-147">microsoft.graph.ediscovery.exportOptions</span><span class="sxs-lookup"><span data-stu-id="0fd6b-147">microsoft.graph.ediscovery.exportOptions</span></span>| <span data-ttu-id="0fd6b-148">Параметры, предусмотренные для экспорта.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-148">The options provided for the export.</span></span> <span data-ttu-id="0fd6b-149">Дополнительные сведения см. в [обзореSet: экспорт.](../api/ediscovery-reviewset-export.md)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-149">See [reviewSet: export](../api/ediscovery-reviewset-export.md) for more details.</span></span> <span data-ttu-id="0fd6b-150">Возможные значения: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-150">Possible values are: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span></span>|
|<span data-ttu-id="0fd6b-151">exportStructure</span><span class="sxs-lookup"><span data-stu-id="0fd6b-151">exportStructure</span></span>|<span data-ttu-id="0fd6b-152">microsoft.graph.ediscovery.exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="0fd6b-152">microsoft.graph.ediscovery.exportFileStructure</span></span>|<span data-ttu-id="0fd6b-153">Параметры, которые указывают структуру экспорта.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-153">The options provided that specify the structure of the export.</span></span> <span data-ttu-id="0fd6b-154">Дополнительные сведения см. в [обзореSet: экспорт.](../api/ediscovery-reviewset-export.md)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-154">See [reviewSet: export](../api/ediscovery-reviewset-export.md) for more details.</span></span> <span data-ttu-id="0fd6b-155">Возможные значения: `none`, `directory`, `pst`.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-155">Possible values are: `none`, `directory`, `pst`.</span></span>|
|<span data-ttu-id="0fd6b-156">id</span><span class="sxs-lookup"><span data-stu-id="0fd6b-156">id</span></span>|<span data-ttu-id="0fd6b-157">String</span><span class="sxs-lookup"><span data-stu-id="0fd6b-157">String</span></span>| <span data-ttu-id="0fd6b-158">ID для операции.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-158">The ID for the operation.</span></span> <span data-ttu-id="0fd6b-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-159">Read-only.</span></span> <span data-ttu-id="0fd6b-160">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0fd6b-160">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="0fd6b-161">outputName</span><span class="sxs-lookup"><span data-stu-id="0fd6b-161">outputName</span></span>|<span data-ttu-id="0fd6b-162">String</span><span class="sxs-lookup"><span data-stu-id="0fd6b-162">String</span></span>| <span data-ttu-id="0fd6b-163">Имя, предоставленное для экспорта.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-163">The name provided for the export.</span></span>|
|<span data-ttu-id="0fd6b-164">percentProgress</span><span class="sxs-lookup"><span data-stu-id="0fd6b-164">percentProgress</span></span>|<span data-ttu-id="0fd6b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0fd6b-165">Int32</span></span>| <span data-ttu-id="0fd6b-166">Ход операции.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-166">The progress of the operation.</span></span> <span data-ttu-id="0fd6b-167">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-167">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="0fd6b-168">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0fd6b-168">resultInfo</span></span>|[<span data-ttu-id="0fd6b-169">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0fd6b-169">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="0fd6b-170">Содержит сведения о результатах, характерных для успешного и неудачного сбоя.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-170">Contains success and failure-specific result information.</span></span> <span data-ttu-id="0fd6b-171">Унаследованный от [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-171">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="0fd6b-172">status</span><span class="sxs-lookup"><span data-stu-id="0fd6b-172">status</span></span>|[<span data-ttu-id="0fd6b-173">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="0fd6b-173">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="0fd6b-174">Состояние операции дела.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-174">The status of the case operation.</span></span> <span data-ttu-id="0fd6b-175">Наследуется [от caseOperation](../resources/ediscovery-caseoperation.md).</span><span class="sxs-lookup"><span data-stu-id="0fd6b-175">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="0fd6b-176">Возможные значения: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-176">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="exportoptions-values"></a><span data-ttu-id="0fd6b-177">Значения exportOptions</span><span class="sxs-lookup"><span data-stu-id="0fd6b-177">exportOptions values</span></span>

|<span data-ttu-id="0fd6b-178">Member</span><span class="sxs-lookup"><span data-stu-id="0fd6b-178">Member</span></span>| <span data-ttu-id="0fd6b-179">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd6b-179">Description</span></span> |
|:---|:---|
|<span data-ttu-id="0fd6b-180">originalFiles</span><span class="sxs-lookup"><span data-stu-id="0fd6b-180">originalFiles</span></span>| <span data-ttu-id="0fd6b-181">Включи копии исходных файлов — исключить этот параметр при создании отчетов</span><span class="sxs-lookup"><span data-stu-id="0fd6b-181">Include copies of the original files - exclude this option when generating reports only</span></span> |
|<span data-ttu-id="0fd6b-182">текст</span><span class="sxs-lookup"><span data-stu-id="0fd6b-182">text</span></span>| <span data-ttu-id="0fd6b-183">Включай необработанные извлеченные текстовые файлы для каждого документа.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-183">Include raw extracted text files for each document.</span></span> |
|<span data-ttu-id="0fd6b-184">pdfReplacement</span><span class="sxs-lookup"><span data-stu-id="0fd6b-184">pdfReplacement</span></span>| <span data-ttu-id="0fd6b-185">Если во время проверки создаются отредактированные PDF-файлы, эти файлы доступны для экспорта.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-185">If redacted PDF files are generated during review, these files are available for export.</span></span> <span data-ttu-id="0fd6b-186">Вы можете экспортировать отредактировали PDFs вместо исходных родных файлов, включив этот параметр.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-186">You can choose to export the redacted PDFs instead of the original native files by including this option.</span></span> |
|<span data-ttu-id="0fd6b-187">fileInfo</span><span class="sxs-lookup"><span data-stu-id="0fd6b-187">fileInfo</span></span>| <span data-ttu-id="0fd6b-188">Включай летний файл и файл нагрузки — это всегда должно быть включено.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-188">Include the summery and load file - this should always be included.</span></span> |
|<span data-ttu-id="0fd6b-189">tags</span><span class="sxs-lookup"><span data-stu-id="0fd6b-189">tags</span></span>| <span data-ttu-id="0fd6b-190">Включай теги документов, которые были применены во время проверки в файле нагрузки.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-190">Include document tags that were applied during review in the load file.</span></span> |

### <a name="exportfilestructure-values"></a><span data-ttu-id="0fd6b-191">значения exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="0fd6b-191">exportFileStructure values</span></span>

|<span data-ttu-id="0fd6b-192">Member</span><span class="sxs-lookup"><span data-stu-id="0fd6b-192">Member</span></span>| <span data-ttu-id="0fd6b-193">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd6b-193">Description</span></span> |
|:---|:---|
|<span data-ttu-id="0fd6b-194">каталог</span><span class="sxs-lookup"><span data-stu-id="0fd6b-194">directory</span></span>| <span data-ttu-id="0fd6b-195">Карты с конденсаторной структурой каталогов, обычно используемой средствами eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-195">Maps to the condensed directory structure commonly used by eDiscovery tools.</span></span> <span data-ttu-id="0fd6b-196">Все файлы экспортируются в корневой файл под названием NativeFiles.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-196">All files are exported to a root file called NativeFiles.</span></span> |
|<span data-ttu-id="0fd6b-197">pST</span><span class="sxs-lookup"><span data-stu-id="0fd6b-197">pst</span></span>| <span data-ttu-id="0fd6b-198">Сообщения электронной почты хранятся в PSTs, а документы с сайтов хранятся в папках, которые представляют исходную структуру папки.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-198">Emails are stored in PSTs while documents from sites are stored in folders that represent the original native folder structure.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0fd6b-199">Связи</span><span class="sxs-lookup"><span data-stu-id="0fd6b-199">Relationships</span></span>

|<span data-ttu-id="0fd6b-200">Связь</span><span class="sxs-lookup"><span data-stu-id="0fd6b-200">Relationship</span></span>|<span data-ttu-id="0fd6b-201">Тип</span><span class="sxs-lookup"><span data-stu-id="0fd6b-201">Type</span></span>|<span data-ttu-id="0fd6b-202">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd6b-202">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fd6b-203">reviewSet</span><span class="sxs-lookup"><span data-stu-id="0fd6b-203">reviewSet</span></span>|[<span data-ttu-id="0fd6b-204">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="0fd6b-204">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md)| <span data-ttu-id="0fd6b-205">В обзоре установлено, из него экспортируется контент.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-205">The review set the content is being exported from.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0fd6b-206">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0fd6b-206">JSON representation</span></span>

<span data-ttu-id="0fd6b-207">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-207">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseExportOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseExportOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "outputName": "String",
  "description": "String",
  "outputFolderId": "String",
  "azureBlobContainer": "String",
  "azureBlobToken": "String",
  "exportOptions": "String",
  "exportStructure": "String"
}
```
