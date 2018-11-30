---
title: Тип ресурса fileSecurityState
description: Содержит сведения о файле (не процесса), связанные с оповещение.
ms.openlocfilehash: d1358d7fe0d5565845201781e32b3da14a89f412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028183"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="1e8c3-103">Тип ресурса fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="1e8c3-103">fileSecurityState resource type</span></span>

<span data-ttu-id="1e8c3-104">Содержит сведения о файле (не процесса), связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="1e8c3-104">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="1e8c3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e8c3-105">Properties</span></span>

| <span data-ttu-id="1e8c3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e8c3-106">Property</span></span>   | <span data-ttu-id="1e8c3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1e8c3-107">Type</span></span>|<span data-ttu-id="1e8c3-108">Description</span><span class="sxs-lookup"><span data-stu-id="1e8c3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e8c3-109">fileHash</span><span class="sxs-lookup"><span data-stu-id="1e8c3-109">fileHash</span></span>|[<span data-ttu-id="1e8c3-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="1e8c3-110">fileHash</span></span>](filehash.md)|<span data-ttu-id="1e8c3-111">Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="1e8c3-111">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="1e8c3-112">name</span><span class="sxs-lookup"><span data-stu-id="1e8c3-112">name</span></span>|<span data-ttu-id="1e8c3-113">String</span><span class="sxs-lookup"><span data-stu-id="1e8c3-113">String</span></span>|<span data-ttu-id="1e8c3-114">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="1e8c3-114">File name (without path).</span></span>|
|<span data-ttu-id="1e8c3-115">path</span><span class="sxs-lookup"><span data-stu-id="1e8c3-115">path</span></span>|<span data-ttu-id="1e8c3-116">String</span><span class="sxs-lookup"><span data-stu-id="1e8c3-116">String</span></span>|<span data-ttu-id="1e8c3-117">Полный путь к файлу файл/файл изображения.</span><span class="sxs-lookup"><span data-stu-id="1e8c3-117">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="1e8c3-118">riskScore</span><span class="sxs-lookup"><span data-stu-id="1e8c3-118">riskScore</span></span>|<span data-ttu-id="1e8c3-119">String</span><span class="sxs-lookup"><span data-stu-id="1e8c3-119">String</span></span>|<span data-ttu-id="1e8c3-120">Поставщик создан/вычисляется риск показатель файл оповещений.</span><span class="sxs-lookup"><span data-stu-id="1e8c3-120">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="1e8c3-121">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="1e8c3-121">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e8c3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e8c3-122">JSON representation</span></span>

<span data-ttu-id="1e8c3-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e8c3-123">The following is a JSON representation of the resource.</span></span>

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