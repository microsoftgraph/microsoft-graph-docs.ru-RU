---
title: Тип ресурса Аттрибутемаппингпараметерсчема
description: Описывает один параметр, используемый в Аттрибутемаппингфунктионсчема.
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582229"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="8c1c7-103">Тип ресурса Аттрибутемаппингпараметерсчема</span><span class="sxs-lookup"><span data-stu-id="8c1c7-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c1c7-104">Описывает один параметр, используемый в [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="8c1c7-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8c1c7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c1c7-105">Properties</span></span>

| <span data-ttu-id="8c1c7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c1c7-106">Property</span></span>                   | <span data-ttu-id="8c1c7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8c1c7-107">Type</span></span>                      | <span data-ttu-id="8c1c7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8c1c7-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="8c1c7-109">Алловмултиплеоккурренцес</span><span class="sxs-lookup"><span data-stu-id="8c1c7-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="8c1c7-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c1c7-110">Boolean</span></span>                   |<span data-ttu-id="8c1c7-111">Данный параметр может быть указан несколько раз (например, с несколькими входными строками в `Concatenate(string,string,...)` функции).</span><span class="sxs-lookup"><span data-stu-id="8c1c7-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="8c1c7-112">name</span><span class="sxs-lookup"><span data-stu-id="8c1c7-112">name</span></span>                        |<span data-ttu-id="8c1c7-113">String</span><span class="sxs-lookup"><span data-stu-id="8c1c7-113">String</span></span>                    |<span data-ttu-id="8c1c7-114">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="8c1c7-114">Parameter name.</span></span> |
|<span data-ttu-id="8c1c7-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8c1c7-115">required</span></span>                    |<span data-ttu-id="8c1c7-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c1c7-116">Boolean</span></span>                   |<span data-ttu-id="8c1c7-117">`true`значение, если параметр является обязательным; в `false`противном случае.</span><span class="sxs-lookup"><span data-stu-id="8c1c7-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="8c1c7-118">type</span><span class="sxs-lookup"><span data-stu-id="8c1c7-118">type</span></span>                        |<span data-ttu-id="8c1c7-119">String</span><span class="sxs-lookup"><span data-stu-id="8c1c7-119">String</span></span>                    |<span data-ttu-id="8c1c7-120">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="8c1c7-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="8c1c7-121">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="8c1c7-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c1c7-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c1c7-122">JSON representation</span></span>

<span data-ttu-id="8c1c7-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c1c7-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingparameterschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
