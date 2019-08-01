---
title: Тип ресурса объекта filesecuritystate
description: Содержит сведения о файле (не процессу), связанном с предупреждением.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6e6f30625412022006d88179e3192b1463c797c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032496"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="623e4-103">Тип ресурса объекта filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="623e4-103">fileSecurityState resource type</span></span>

<span data-ttu-id="623e4-104">Содержит сведения о файле (не процессу), связанном с предупреждением.</span><span class="sxs-lookup"><span data-stu-id="623e4-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="623e4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="623e4-105">Properties</span></span>

| <span data-ttu-id="623e4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="623e4-106">Property</span></span>   | <span data-ttu-id="623e4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="623e4-107">Type</span></span>|<span data-ttu-id="623e4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="623e4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="623e4-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="623e4-109">fileHash</span></span>|[<span data-ttu-id="623e4-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="623e4-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="623e4-111">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="623e4-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="623e4-112">name</span><span class="sxs-lookup"><span data-stu-id="623e4-112">name</span></span>|<span data-ttu-id="623e4-113">String</span><span class="sxs-lookup"><span data-stu-id="623e4-113">String</span></span>|<span data-ttu-id="623e4-114">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="623e4-114">File name (without path).</span></span>|
|<span data-ttu-id="623e4-115">path</span><span class="sxs-lookup"><span data-stu-id="623e4-115">path</span></span>|<span data-ttu-id="623e4-116">String</span><span class="sxs-lookup"><span data-stu-id="623e4-116">String</span></span>|<span data-ttu-id="623e4-117">Полный путь к файлу или файлу imageFile.</span><span class="sxs-lookup"><span data-stu-id="623e4-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="623e4-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="623e4-118">riskScore</span></span>|<span data-ttu-id="623e4-119">String</span><span class="sxs-lookup"><span data-stu-id="623e4-119">String</span></span>|<span data-ttu-id="623e4-120">Созданный поставщиком/вычисляемый показатель риска для файла оповещений.</span><span class="sxs-lookup"><span data-stu-id="623e4-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="623e4-121">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="623e4-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="623e4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="623e4-122">JSON representation</span></span>

<span data-ttu-id="623e4-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="623e4-123">The following is a JSON representation of the resource.</span></span>

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
