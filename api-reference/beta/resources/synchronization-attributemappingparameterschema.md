---
title: Тип ресурса Аттрибутемаппингпараметерсчема
description: Описывает один параметр, используемый в Аттрибутемаппингфунктионсчема.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14be19389d7c84c3e1a212239f2ba9e414927254
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964846"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="ac33e-103">Тип ресурса Аттрибутемаппингпараметерсчема</span><span class="sxs-lookup"><span data-stu-id="ac33e-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac33e-104">Описывает один параметр, используемый в [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="ac33e-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ac33e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac33e-105">Properties</span></span>

| <span data-ttu-id="ac33e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac33e-106">Property</span></span>                   | <span data-ttu-id="ac33e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ac33e-107">Type</span></span>                      | <span data-ttu-id="ac33e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ac33e-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="ac33e-109">Алловмултиплеоккурренцес</span><span class="sxs-lookup"><span data-stu-id="ac33e-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="ac33e-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac33e-110">Boolean</span></span>                   |<span data-ttu-id="ac33e-111">Данный параметр может быть указан несколько раз (например, с несколькими входными строками в `Concatenate(string,string,...)` функции).</span><span class="sxs-lookup"><span data-stu-id="ac33e-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="ac33e-112">name</span><span class="sxs-lookup"><span data-stu-id="ac33e-112">name</span></span>                        |<span data-ttu-id="ac33e-113">String</span><span class="sxs-lookup"><span data-stu-id="ac33e-113">String</span></span>                    |<span data-ttu-id="ac33e-114">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="ac33e-114">Parameter name.</span></span> |
|<span data-ttu-id="ac33e-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="ac33e-115">required</span></span>                    |<span data-ttu-id="ac33e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac33e-116">Boolean</span></span>                   |<span data-ttu-id="ac33e-117">`true`значение, если параметр является обязательным; в `false`противном случае.</span><span class="sxs-lookup"><span data-stu-id="ac33e-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="ac33e-118">type</span><span class="sxs-lookup"><span data-stu-id="ac33e-118">type</span></span>                        |<span data-ttu-id="ac33e-119">String</span><span class="sxs-lookup"><span data-stu-id="ac33e-119">String</span></span>                    |<span data-ttu-id="ac33e-120">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="ac33e-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="ac33e-121">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="ac33e-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac33e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac33e-122">JSON representation</span></span>

<span data-ttu-id="ac33e-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac33e-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
