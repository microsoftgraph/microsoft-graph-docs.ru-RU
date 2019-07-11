---
title: Тип ресурса Аттрибутемаппингпараметерсчема
description: Описывает один параметр, используемый в Аттрибутемаппингфунктионсчема.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8624851d37f475df66ec51f1951ebbbe1ea97a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620271"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="400e0-103">Тип ресурса Аттрибутемаппингпараметерсчема</span><span class="sxs-lookup"><span data-stu-id="400e0-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="400e0-104">Описывает один параметр, используемый в [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="400e0-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="400e0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="400e0-105">Properties</span></span>

| <span data-ttu-id="400e0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="400e0-106">Property</span></span>                   | <span data-ttu-id="400e0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="400e0-107">Type</span></span>                      | <span data-ttu-id="400e0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="400e0-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="400e0-109">Алловмултиплеоккурренцес</span><span class="sxs-lookup"><span data-stu-id="400e0-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="400e0-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="400e0-110">Boolean</span></span>                   |<span data-ttu-id="400e0-111">Данный параметр может быть указан несколько раз (например, с несколькими входными строками в `Concatenate(string,string,...)` функции).</span><span class="sxs-lookup"><span data-stu-id="400e0-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="400e0-112">name</span><span class="sxs-lookup"><span data-stu-id="400e0-112">name</span></span>                        |<span data-ttu-id="400e0-113">String</span><span class="sxs-lookup"><span data-stu-id="400e0-113">String</span></span>                    |<span data-ttu-id="400e0-114">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="400e0-114">Parameter name.</span></span> |
|<span data-ttu-id="400e0-115">Обязательный</span><span class="sxs-lookup"><span data-stu-id="400e0-115">required</span></span>                    |<span data-ttu-id="400e0-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="400e0-116">Boolean</span></span>                   |<span data-ttu-id="400e0-117">`true`значение, если параметр является обязательным; в `false`противном случае.</span><span class="sxs-lookup"><span data-stu-id="400e0-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="400e0-118">type</span><span class="sxs-lookup"><span data-stu-id="400e0-118">type</span></span>                        |<span data-ttu-id="400e0-119">String</span><span class="sxs-lookup"><span data-stu-id="400e0-119">String</span></span>                    |<span data-ttu-id="400e0-120">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="400e0-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="400e0-121">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="400e0-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="400e0-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="400e0-122">JSON representation</span></span>

<span data-ttu-id="400e0-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="400e0-123">The following is a JSON representation of the resource.</span></span>

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
