---
title: Тип ресурса fileSecurityState
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: cbf535dd6b30387afbe361389fa6bcfca1fc68fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082005"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="9d7f3-104">Тип ресурса fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="9d7f3-104">fileSecurityState resource type</span></span>

 > <span data-ttu-id="9d7f3-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d7f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d7f3-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d7f3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d7f3-107">Содержит сведения о файле (не процесса), связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="9d7f3-107">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="9d7f3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d7f3-108">Properties</span></span>

| <span data-ttu-id="9d7f3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d7f3-109">Property</span></span>   | <span data-ttu-id="9d7f3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9d7f3-110">Type</span></span>|<span data-ttu-id="9d7f3-111">Description</span><span class="sxs-lookup"><span data-stu-id="9d7f3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d7f3-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="9d7f3-112">fileHash</span></span>|[<span data-ttu-id="9d7f3-113">fileHash</span><span class="sxs-lookup"><span data-stu-id="9d7f3-113">fileHash</span></span>](filehash.md)|<span data-ttu-id="9d7f3-114">Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="9d7f3-114">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="9d7f3-115">name</span><span class="sxs-lookup"><span data-stu-id="9d7f3-115">name</span></span>|<span data-ttu-id="9d7f3-116">String</span><span class="sxs-lookup"><span data-stu-id="9d7f3-116">String</span></span>|<span data-ttu-id="9d7f3-117">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="9d7f3-117">File name (without path).</span></span>|
|<span data-ttu-id="9d7f3-118">path</span><span class="sxs-lookup"><span data-stu-id="9d7f3-118">path</span></span>|<span data-ttu-id="9d7f3-119">String</span><span class="sxs-lookup"><span data-stu-id="9d7f3-119">String</span></span>|<span data-ttu-id="9d7f3-120">Полный путь к файлу файл/файл изображения.</span><span class="sxs-lookup"><span data-stu-id="9d7f3-120">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="9d7f3-121">riskScore</span><span class="sxs-lookup"><span data-stu-id="9d7f3-121">riskScore</span></span>|<span data-ttu-id="9d7f3-122">String</span><span class="sxs-lookup"><span data-stu-id="9d7f3-122">String</span></span>|<span data-ttu-id="9d7f3-123">Поставщик создан/вычисляется риск показатель файл оповещений.</span><span class="sxs-lookup"><span data-stu-id="9d7f3-123">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="9d7f3-124">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="9d7f3-124">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d7f3-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d7f3-125">JSON representation</span></span>

<span data-ttu-id="9d7f3-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d7f3-126">The following is a JSON representation of the resource.</span></span>

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