---
title: Тип ресурса attributeMappingParameterSchema
description: Описывает один параметр, используемый в attributeMappingFunctionSchema.
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529952"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="c05c8-103">Тип ресурса attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="c05c8-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c05c8-104">Описывает один параметр, используемый в [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="c05c8-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c05c8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c05c8-105">Properties</span></span>

| <span data-ttu-id="c05c8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c05c8-106">Property</span></span>                   | <span data-ttu-id="c05c8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c05c8-107">Type</span></span>                      | <span data-ttu-id="c05c8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c05c8-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="c05c8-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="c05c8-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="c05c8-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="c05c8-110">Boolean</span></span>                   |<span data-ttu-id="c05c8-111">Данному параметру можно указать несколько раз (например нескольких входных данных строки в `Concatenate(string,string,...)` функция).</span><span class="sxs-lookup"><span data-stu-id="c05c8-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="c05c8-112">name</span><span class="sxs-lookup"><span data-stu-id="c05c8-112">name</span></span>                        |<span data-ttu-id="c05c8-113">String</span><span class="sxs-lookup"><span data-stu-id="c05c8-113">String</span></span>                    |<span data-ttu-id="c05c8-114">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c05c8-114">Parameter name.</span></span> |
|<span data-ttu-id="c05c8-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="c05c8-115">required</span></span>                    |<span data-ttu-id="c05c8-116">Логическое</span><span class="sxs-lookup"><span data-stu-id="c05c8-116">Boolean</span></span>                   |<span data-ttu-id="c05c8-117">`true`Если параметр является обязательным; в противном случае `false`.</span><span class="sxs-lookup"><span data-stu-id="c05c8-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="c05c8-118">type</span><span class="sxs-lookup"><span data-stu-id="c05c8-118">type</span></span>                        |<span data-ttu-id="c05c8-119">String</span><span class="sxs-lookup"><span data-stu-id="c05c8-119">String</span></span>                    |<span data-ttu-id="c05c8-120">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="c05c8-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="c05c8-121">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="c05c8-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c05c8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c05c8-122">JSON representation</span></span>

<span data-ttu-id="c05c8-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c05c8-123">The following is a JSON representation of the resource.</span></span>

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
