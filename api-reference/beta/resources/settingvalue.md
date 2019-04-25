---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
ms.openlocfilehash: aa30fd61c1498be08be4d87175d18015c58323ba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584109"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="fd422-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="fd422-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd422-104">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="fd422-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="fd422-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd422-105">Properties</span></span>
| <span data-ttu-id="fd422-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd422-106">Property</span></span>     | <span data-ttu-id="fd422-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fd422-107">Type</span></span>   |<span data-ttu-id="fd422-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fd422-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd422-109">name</span><span class="sxs-lookup"><span data-stu-id="fd422-109">name</span></span>|<span data-ttu-id="fd422-110">string</span><span class="sxs-lookup"><span data-stu-id="fd422-110">string</span></span>|<span data-ttu-id="fd422-111">Имя параметра (как определено в Директорисеттингтемплате).</span><span class="sxs-lookup"><span data-stu-id="fd422-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="fd422-112">value</span><span class="sxs-lookup"><span data-stu-id="fd422-112">value</span></span>|<span data-ttu-id="fd422-113">string</span><span class="sxs-lookup"><span data-stu-id="fd422-113">string</span></span>|<span data-ttu-id="fd422-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="fd422-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd422-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd422-115">JSON representation</span></span>

<span data-ttu-id="fd422-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd422-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/settingvalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
