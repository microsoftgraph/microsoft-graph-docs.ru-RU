---
title: Тип ресурса fileSecurityState
description: Содержит сведения о файле (не процесса), связанные с оповещение.
localization_priority: Normal
ms.openlocfilehash: 14ffa41b395bde04972f0af0436297aa4d038524
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894098"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="4720a-103">Тип ресурса fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="4720a-103">fileSecurityState resource type</span></span>

<span data-ttu-id="4720a-104">Содержит сведения о файле (не процесса), связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="4720a-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="4720a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4720a-105">Properties</span></span>

| <span data-ttu-id="4720a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4720a-106">Property</span></span>   | <span data-ttu-id="4720a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4720a-107">Type</span></span>|<span data-ttu-id="4720a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4720a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4720a-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="4720a-109">fileHash</span></span>|[<span data-ttu-id="4720a-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="4720a-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="4720a-111">Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="4720a-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="4720a-112">name</span><span class="sxs-lookup"><span data-stu-id="4720a-112">name</span></span>|<span data-ttu-id="4720a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="4720a-113">String</span></span>|<span data-ttu-id="4720a-114">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="4720a-114">File name (without path).</span></span>|
|<span data-ttu-id="4720a-115">path</span><span class="sxs-lookup"><span data-stu-id="4720a-115">path</span></span>|<span data-ttu-id="4720a-116">String</span><span class="sxs-lookup"><span data-stu-id="4720a-116">String</span></span>|<span data-ttu-id="4720a-117">Полный путь к файлу файл/файл изображения.</span><span class="sxs-lookup"><span data-stu-id="4720a-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="4720a-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="4720a-118">riskScore</span></span>|<span data-ttu-id="4720a-119">Строка</span><span class="sxs-lookup"><span data-stu-id="4720a-119">String</span></span>|<span data-ttu-id="4720a-120">Поставщик создан/вычисляется риск показатель файл оповещений.</span><span class="sxs-lookup"><span data-stu-id="4720a-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="4720a-121">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="4720a-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4720a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4720a-122">JSON representation</span></span>

<span data-ttu-id="4720a-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4720a-123">The following is a JSON representation of the resource.</span></span>

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
