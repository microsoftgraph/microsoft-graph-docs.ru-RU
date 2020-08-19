---
title: Тип ресурса объекта filesecuritystate
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: e030ce95ef2b8c5f1af5424bfdd0e727f2d3e2f6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806543"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="3706d-104">Тип ресурса объекта filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="3706d-104">fileSecurityState resource type</span></span>

<span data-ttu-id="3706d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3706d-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3706d-106">Содержит сведения о файле (не процессу), связанном с предупреждением.</span><span class="sxs-lookup"><span data-stu-id="3706d-106">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="3706d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3706d-107">Properties</span></span>

| <span data-ttu-id="3706d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3706d-108">Property</span></span>   | <span data-ttu-id="3706d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3706d-109">Type</span></span>|<span data-ttu-id="3706d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3706d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3706d-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="3706d-111">fileHash</span></span>|[<span data-ttu-id="3706d-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="3706d-112">fileHash</span></span>](filehash.md)|<span data-ttu-id="3706d-113">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="3706d-113">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="3706d-114">name</span><span class="sxs-lookup"><span data-stu-id="3706d-114">name</span></span>|<span data-ttu-id="3706d-115">String</span><span class="sxs-lookup"><span data-stu-id="3706d-115">String</span></span>|<span data-ttu-id="3706d-116">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="3706d-116">File name (without path).</span></span>|
|<span data-ttu-id="3706d-117">path</span><span class="sxs-lookup"><span data-stu-id="3706d-117">path</span></span>|<span data-ttu-id="3706d-118">String</span><span class="sxs-lookup"><span data-stu-id="3706d-118">String</span></span>|<span data-ttu-id="3706d-119">Полный путь к файлу или файлу imageFile.</span><span class="sxs-lookup"><span data-stu-id="3706d-119">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="3706d-120">riskScore</span><span class="sxs-lookup"><span data-stu-id="3706d-120">riskScore</span></span>|<span data-ttu-id="3706d-121">String</span><span class="sxs-lookup"><span data-stu-id="3706d-121">String</span></span>|<span data-ttu-id="3706d-122">Созданный поставщиком/вычисляемый показатель риска для файла оповещений.</span><span class="sxs-lookup"><span data-stu-id="3706d-122">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="3706d-123">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="3706d-123">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3706d-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3706d-124">JSON representation</span></span>

<span data-ttu-id="3706d-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3706d-125">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
