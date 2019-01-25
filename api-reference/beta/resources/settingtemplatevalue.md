---
title: Тип ресурса settingTemplateValue
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528013"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="e589b-103">Тип ресурса settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="e589b-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e589b-104">Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.</span><span class="sxs-lookup"><span data-stu-id="e589b-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="e589b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e589b-105">Properties</span></span>
| <span data-ttu-id="e589b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e589b-106">Property</span></span>     | <span data-ttu-id="e589b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e589b-107">Type</span></span>   |<span data-ttu-id="e589b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e589b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e589b-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="e589b-109">defaultValue</span></span>|<span data-ttu-id="e589b-110">string</span><span class="sxs-lookup"><span data-stu-id="e589b-110">string</span></span>|<span data-ttu-id="e589b-111">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="e589b-111">Default value for the setting.</span></span> <span data-ttu-id="e589b-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e589b-112">Read-only.</span></span>|
|<span data-ttu-id="e589b-113">description</span><span class="sxs-lookup"><span data-stu-id="e589b-113">description</span></span>|<span data-ttu-id="e589b-114">строка</span><span class="sxs-lookup"><span data-stu-id="e589b-114">string</span></span>|<span data-ttu-id="e589b-115">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="e589b-115">Description of the setting.</span></span> <span data-ttu-id="e589b-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e589b-116">Read-only.</span></span>|
|<span data-ttu-id="e589b-117">name</span><span class="sxs-lookup"><span data-stu-id="e589b-117">name</span></span>|<span data-ttu-id="e589b-118">string</span><span class="sxs-lookup"><span data-stu-id="e589b-118">string</span></span>|<span data-ttu-id="e589b-119">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="e589b-119">Name of the setting.</span></span> <span data-ttu-id="e589b-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e589b-120">Read-only.</span></span>|
|<span data-ttu-id="e589b-121">type</span><span class="sxs-lookup"><span data-stu-id="e589b-121">type</span></span>|<span data-ttu-id="e589b-122">string</span><span class="sxs-lookup"><span data-stu-id="e589b-122">string</span></span>|<span data-ttu-id="e589b-123">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="e589b-123">Type of the setting.</span></span> <span data-ttu-id="e589b-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e589b-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e589b-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e589b-125">JSON representation</span></span>

<span data-ttu-id="e589b-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e589b-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/settingtemplatevalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
