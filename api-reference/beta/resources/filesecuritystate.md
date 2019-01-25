---
title: Тип ресурса fileSecurityState
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 485addfda2707c8848c44c839f9593378943f327
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526958"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="fea4a-104">Тип ресурса fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="fea4a-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fea4a-105">Содержит сведения о файле (не процесса), связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="fea4a-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="fea4a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fea4a-106">Properties</span></span>

| <span data-ttu-id="fea4a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fea4a-107">Property</span></span>   | <span data-ttu-id="fea4a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fea4a-108">Type</span></span>|<span data-ttu-id="fea4a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fea4a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fea4a-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="fea4a-110">fileHash</span></span>|[<span data-ttu-id="fea4a-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="fea4a-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="fea4a-112">Сложный тип, содержащий файл хэш-значений (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="fea4a-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="fea4a-113">name</span><span class="sxs-lookup"><span data-stu-id="fea4a-113">name</span></span>|<span data-ttu-id="fea4a-114">String</span><span class="sxs-lookup"><span data-stu-id="fea4a-114">String</span></span>|<span data-ttu-id="fea4a-115">Имя файла (без пути).</span><span class="sxs-lookup"><span data-stu-id="fea4a-115">File name (without path).</span></span>|
|<span data-ttu-id="fea4a-116">path</span><span class="sxs-lookup"><span data-stu-id="fea4a-116">path</span></span>|<span data-ttu-id="fea4a-117">String</span><span class="sxs-lookup"><span data-stu-id="fea4a-117">String</span></span>|<span data-ttu-id="fea4a-118">Полный путь к файлу файл/файл изображения.</span><span class="sxs-lookup"><span data-stu-id="fea4a-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="fea4a-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="fea4a-119">riskScore</span></span>|<span data-ttu-id="fea4a-120">String</span><span class="sxs-lookup"><span data-stu-id="fea4a-120">String</span></span>|<span data-ttu-id="fea4a-121">Поставщик создан/вычисляется риск показатель файл оповещений.</span><span class="sxs-lookup"><span data-stu-id="fea4a-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="fea4a-122">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="fea4a-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fea4a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fea4a-123">JSON representation</span></span>

<span data-ttu-id="fea4a-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fea4a-124">The following is a JSON representation of the resource.</span></span>

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
