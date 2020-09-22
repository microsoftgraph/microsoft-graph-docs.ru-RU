---
title: Тип ресурса объекта filesecuritystate
description: Содержит сведения о файле (не процессу), связанном с предупреждением.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d636350237c34464b557a970e3bbf121d50de88a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018370"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="36ab7-103">Тип ресурса объекта filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="36ab7-103">fileSecurityState resource type</span></span>

<span data-ttu-id="36ab7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36ab7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36ab7-105">Содержит сведения о файле (не процессу), связанном с предупреждением.</span><span class="sxs-lookup"><span data-stu-id="36ab7-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="36ab7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="36ab7-106">Properties</span></span>

| <span data-ttu-id="36ab7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="36ab7-107">Property</span></span>   | <span data-ttu-id="36ab7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="36ab7-108">Type</span></span>|<span data-ttu-id="36ab7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36ab7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36ab7-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="36ab7-110">fileHash</span></span>|[<span data-ttu-id="36ab7-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="36ab7-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="36ab7-112">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="36ab7-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="36ab7-113">name</span><span class="sxs-lookup"><span data-stu-id="36ab7-113">name</span></span>|<span data-ttu-id="36ab7-114">String</span><span class="sxs-lookup"><span data-stu-id="36ab7-114">String</span></span>|<span data-ttu-id="36ab7-115">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="36ab7-115">File name (without path).</span></span>|
|<span data-ttu-id="36ab7-116">path</span><span class="sxs-lookup"><span data-stu-id="36ab7-116">path</span></span>|<span data-ttu-id="36ab7-117">String</span><span class="sxs-lookup"><span data-stu-id="36ab7-117">String</span></span>|<span data-ttu-id="36ab7-118">Полный путь к файлу или файлу imageFile.</span><span class="sxs-lookup"><span data-stu-id="36ab7-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="36ab7-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="36ab7-119">riskScore</span></span>|<span data-ttu-id="36ab7-120">String</span><span class="sxs-lookup"><span data-stu-id="36ab7-120">String</span></span>|<span data-ttu-id="36ab7-121">Созданный поставщиком/вычисляемый показатель риска для файла оповещений.</span><span class="sxs-lookup"><span data-stu-id="36ab7-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="36ab7-122">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="36ab7-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36ab7-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36ab7-123">JSON representation</span></span>

<span data-ttu-id="36ab7-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36ab7-124">The following is a JSON representation of the resource.</span></span>

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

