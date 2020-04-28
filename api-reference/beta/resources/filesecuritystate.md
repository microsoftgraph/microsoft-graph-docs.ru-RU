---
title: Тип ресурса объекта filesecuritystate
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3827562407b0c253c1d5a16ff26071e8500010bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498170"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="8c8b8-104">Тип ресурса объекта filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="8c8b8-104">fileSecurityState resource type</span></span>

<span data-ttu-id="8c8b8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c8b8-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c8b8-106">Содержит сведения о файле (не процессу), связанном с предупреждением.</span><span class="sxs-lookup"><span data-stu-id="8c8b8-106">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="8c8b8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c8b8-107">Properties</span></span>

| <span data-ttu-id="8c8b8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c8b8-108">Property</span></span>   | <span data-ttu-id="8c8b8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8c8b8-109">Type</span></span>|<span data-ttu-id="8c8b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c8b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c8b8-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="8c8b8-111">fileHash</span></span>|[<span data-ttu-id="8c8b8-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="8c8b8-112">fileHash</span></span>](filehash.md)|<span data-ttu-id="8c8b8-113">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="8c8b8-113">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="8c8b8-114">name</span><span class="sxs-lookup"><span data-stu-id="8c8b8-114">name</span></span>|<span data-ttu-id="8c8b8-115">String</span><span class="sxs-lookup"><span data-stu-id="8c8b8-115">String</span></span>|<span data-ttu-id="8c8b8-116">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="8c8b8-116">File name (without path).</span></span>|
|<span data-ttu-id="8c8b8-117">path</span><span class="sxs-lookup"><span data-stu-id="8c8b8-117">path</span></span>|<span data-ttu-id="8c8b8-118">String</span><span class="sxs-lookup"><span data-stu-id="8c8b8-118">String</span></span>|<span data-ttu-id="8c8b8-119">Полный путь к файлу или файлу imageFile.</span><span class="sxs-lookup"><span data-stu-id="8c8b8-119">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="8c8b8-120">riskScore</span><span class="sxs-lookup"><span data-stu-id="8c8b8-120">riskScore</span></span>|<span data-ttu-id="8c8b8-121">String</span><span class="sxs-lookup"><span data-stu-id="8c8b8-121">String</span></span>|<span data-ttu-id="8c8b8-122">Созданный поставщиком/вычисляемый показатель риска для файла оповещений.</span><span class="sxs-lookup"><span data-stu-id="8c8b8-122">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="8c8b8-123">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="8c8b8-123">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c8b8-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c8b8-124">JSON representation</span></span>

<span data-ttu-id="8c8b8-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c8b8-125">The following is a JSON representation of the resource.</span></span>

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
