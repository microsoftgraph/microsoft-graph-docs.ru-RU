---
title: Тип ресурса объекта filesecuritystate
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 485addfda2707c8848c44c839f9593378943f327
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506416"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="f5445-104">Тип ресурса объекта filesecuritystate</span><span class="sxs-lookup"><span data-stu-id="f5445-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5445-105">Содержит сведения о файле (не процессу), связанном с предупреждением.</span><span class="sxs-lookup"><span data-stu-id="f5445-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="f5445-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5445-106">Properties</span></span>

| <span data-ttu-id="f5445-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5445-107">Property</span></span>   | <span data-ttu-id="f5445-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f5445-108">Type</span></span>|<span data-ttu-id="f5445-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f5445-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5445-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="f5445-110">fileHash</span></span>|[<span data-ttu-id="f5445-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="f5445-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="f5445-112">Сложный тип, содержащий хэши файлов (криптография и с учетом расположения).</span><span class="sxs-lookup"><span data-stu-id="f5445-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="f5445-113">name</span><span class="sxs-lookup"><span data-stu-id="f5445-113">name</span></span>|<span data-ttu-id="f5445-114">String</span><span class="sxs-lookup"><span data-stu-id="f5445-114">String</span></span>|<span data-ttu-id="f5445-115">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="f5445-115">File name (without path).</span></span>|
|<span data-ttu-id="f5445-116">path</span><span class="sxs-lookup"><span data-stu-id="f5445-116">path</span></span>|<span data-ttu-id="f5445-117">String</span><span class="sxs-lookup"><span data-stu-id="f5445-117">String</span></span>|<span data-ttu-id="f5445-118">Полный путь к файлу или файлу imageFile.</span><span class="sxs-lookup"><span data-stu-id="f5445-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="f5445-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="f5445-119">riskScore</span></span>|<span data-ttu-id="f5445-120">String</span><span class="sxs-lookup"><span data-stu-id="f5445-120">String</span></span>|<span data-ttu-id="f5445-121">Созданный поставщиком/вычисляемый показатель риска для файла оповещений.</span><span class="sxs-lookup"><span data-stu-id="f5445-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="f5445-122">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="f5445-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5445-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5445-123">JSON representation</span></span>

<span data-ttu-id="f5445-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5445-124">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/filesecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
