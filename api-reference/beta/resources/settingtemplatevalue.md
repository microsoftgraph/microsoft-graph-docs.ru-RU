---
title: Тип ресурса Сеттингтемплатевалуе
description: Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583683"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="09ea0-103">Тип ресурса Сеттингтемплатевалуе</span><span class="sxs-lookup"><span data-stu-id="09ea0-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ea0-104">Представляет определение отдельного параметра шаблона, включая значение по умолчанию, если не создается экземпляр этого параметра.</span><span class="sxs-lookup"><span data-stu-id="09ea0-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="09ea0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="09ea0-105">Properties</span></span>
| <span data-ttu-id="09ea0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="09ea0-106">Property</span></span>     | <span data-ttu-id="09ea0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="09ea0-107">Type</span></span>   |<span data-ttu-id="09ea0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="09ea0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09ea0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="09ea0-109">defaultValue</span></span>|<span data-ttu-id="09ea0-110">string</span><span class="sxs-lookup"><span data-stu-id="09ea0-110">string</span></span>|<span data-ttu-id="09ea0-111">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="09ea0-111">Default value for the setting.</span></span> <span data-ttu-id="09ea0-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09ea0-112">Read-only.</span></span>|
|<span data-ttu-id="09ea0-113">description</span><span class="sxs-lookup"><span data-stu-id="09ea0-113">description</span></span>|<span data-ttu-id="09ea0-114">string</span><span class="sxs-lookup"><span data-stu-id="09ea0-114">string</span></span>|<span data-ttu-id="09ea0-115">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="09ea0-115">Description of the setting.</span></span> <span data-ttu-id="09ea0-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09ea0-116">Read-only.</span></span>|
|<span data-ttu-id="09ea0-117">name</span><span class="sxs-lookup"><span data-stu-id="09ea0-117">name</span></span>|<span data-ttu-id="09ea0-118">строка</span><span class="sxs-lookup"><span data-stu-id="09ea0-118">string</span></span>|<span data-ttu-id="09ea0-119">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="09ea0-119">Name of the setting.</span></span> <span data-ttu-id="09ea0-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09ea0-120">Read-only.</span></span>|
|<span data-ttu-id="09ea0-121">type</span><span class="sxs-lookup"><span data-stu-id="09ea0-121">type</span></span>|<span data-ttu-id="09ea0-122">string</span><span class="sxs-lookup"><span data-stu-id="09ea0-122">string</span></span>|<span data-ttu-id="09ea0-123">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="09ea0-123">Type of the setting.</span></span> <span data-ttu-id="09ea0-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09ea0-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09ea0-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09ea0-125">JSON representation</span></span>

<span data-ttu-id="09ea0-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09ea0-126">Here is a JSON representation of the resource.</span></span>

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
