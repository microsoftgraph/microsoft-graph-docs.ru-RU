---
title: Тип ресурса объекта filesecuritystate
description: Содержит сведения о файле (не процессу), связанном с предупреждением.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564794"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="09e6f-103">Тип ресурса объекта filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="09e6f-103">fileSecurityState resource type</span></span>

<span data-ttu-id="09e6f-104">Содержит сведения о файле (не процессу), связанном с предупреждением.</span><span class="sxs-lookup"><span data-stu-id="09e6f-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="09e6f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="09e6f-105">Properties</span></span>

| <span data-ttu-id="09e6f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="09e6f-106">Property</span></span>   | <span data-ttu-id="09e6f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="09e6f-107">Type</span></span>|<span data-ttu-id="09e6f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="09e6f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09e6f-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="09e6f-109">fileHash</span></span>|[<span data-ttu-id="09e6f-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="09e6f-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="09e6f-111">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="09e6f-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="09e6f-112">name</span><span class="sxs-lookup"><span data-stu-id="09e6f-112">name</span></span>|<span data-ttu-id="09e6f-113">String</span><span class="sxs-lookup"><span data-stu-id="09e6f-113">String</span></span>|<span data-ttu-id="09e6f-114">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="09e6f-114">File name (without path).</span></span>|
|<span data-ttu-id="09e6f-115">path</span><span class="sxs-lookup"><span data-stu-id="09e6f-115">path</span></span>|<span data-ttu-id="09e6f-116">String</span><span class="sxs-lookup"><span data-stu-id="09e6f-116">String</span></span>|<span data-ttu-id="09e6f-117">Полный путь к файлу или файлу imageFile.</span><span class="sxs-lookup"><span data-stu-id="09e6f-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="09e6f-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="09e6f-118">riskScore</span></span>|<span data-ttu-id="09e6f-119">String</span><span class="sxs-lookup"><span data-stu-id="09e6f-119">String</span></span>|<span data-ttu-id="09e6f-120">Созданный поставщиком/вычисляемый показатель риска для файла оповещений.</span><span class="sxs-lookup"><span data-stu-id="09e6f-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="09e6f-121">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="09e6f-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09e6f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09e6f-122">JSON representation</span></span>

<span data-ttu-id="09e6f-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09e6f-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
