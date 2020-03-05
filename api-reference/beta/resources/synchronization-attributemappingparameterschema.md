---
title: Тип ресурса Аттрибутемаппингпараметерсчема
description: Описывает один параметр, используемый в Аттрибутемаппингфунктионсчема.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d4415c6ece2fc9095070eb888ad4bd7bba583d54
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520242"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="44d09-103">Тип ресурса Аттрибутемаппингпараметерсчема</span><span class="sxs-lookup"><span data-stu-id="44d09-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="44d09-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="44d09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44d09-105">Описывает один параметр, используемый в [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="44d09-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="44d09-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="44d09-106">Properties</span></span>

| <span data-ttu-id="44d09-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="44d09-107">Property</span></span>                   | <span data-ttu-id="44d09-108">Тип</span><span class="sxs-lookup"><span data-stu-id="44d09-108">Type</span></span>                      | <span data-ttu-id="44d09-109">Описание</span><span class="sxs-lookup"><span data-stu-id="44d09-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="44d09-110">алловмултиплеоккурренцес</span><span class="sxs-lookup"><span data-stu-id="44d09-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="44d09-111">Логический</span><span class="sxs-lookup"><span data-stu-id="44d09-111">Boolean</span></span>                   |<span data-ttu-id="44d09-112">Данный параметр может быть указан несколько раз (например, с несколькими входными строками в `Concatenate(string,string,...)` функции).</span><span class="sxs-lookup"><span data-stu-id="44d09-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="44d09-113">name</span><span class="sxs-lookup"><span data-stu-id="44d09-113">name</span></span>                        |<span data-ttu-id="44d09-114">String</span><span class="sxs-lookup"><span data-stu-id="44d09-114">String</span></span>                    |<span data-ttu-id="44d09-115">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="44d09-115">Parameter name.</span></span> |
|<span data-ttu-id="44d09-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="44d09-116">required</span></span>                    |<span data-ttu-id="44d09-117">Логический</span><span class="sxs-lookup"><span data-stu-id="44d09-117">Boolean</span></span>                   |<span data-ttu-id="44d09-118">`true`значение, если параметр является обязательным; в `false`противном случае.</span><span class="sxs-lookup"><span data-stu-id="44d09-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="44d09-119">type</span><span class="sxs-lookup"><span data-stu-id="44d09-119">type</span></span>                        |<span data-ttu-id="44d09-120">String</span><span class="sxs-lookup"><span data-stu-id="44d09-120">String</span></span>                    |<span data-ttu-id="44d09-121">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="44d09-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="44d09-122">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="44d09-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44d09-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44d09-123">JSON representation</span></span>

<span data-ttu-id="44d09-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44d09-124">The following is a JSON representation of the resource.</span></span>

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
