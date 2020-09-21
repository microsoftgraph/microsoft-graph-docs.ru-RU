---
title: Тип ресурса Аттрибутемаппингпараметерсчема
description: Описывает один параметр, используемый в Аттрибутемаппингфунктионсчема.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32710c5411f054ad096bdd293a2f7d46e89a6944
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078086"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="5a0f4-103">Тип ресурса Аттрибутемаппингпараметерсчема</span><span class="sxs-lookup"><span data-stu-id="5a0f4-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="5a0f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a0f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a0f4-105">Описывает один параметр, используемый в [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="5a0f4-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a0f4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a0f4-106">Properties</span></span>

| <span data-ttu-id="5a0f4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a0f4-107">Property</span></span>                   | <span data-ttu-id="5a0f4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5a0f4-108">Type</span></span>                      | <span data-ttu-id="5a0f4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a0f4-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="5a0f4-110">алловмултиплеоккурренцес</span><span class="sxs-lookup"><span data-stu-id="5a0f4-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="5a0f4-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a0f4-111">Boolean</span></span>                   |<span data-ttu-id="5a0f4-112">Данный параметр может быть указан несколько раз (например, с несколькими входными строками в `Concatenate(string,string,...)` функции).</span><span class="sxs-lookup"><span data-stu-id="5a0f4-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="5a0f4-113">name</span><span class="sxs-lookup"><span data-stu-id="5a0f4-113">name</span></span>                        |<span data-ttu-id="5a0f4-114">String</span><span class="sxs-lookup"><span data-stu-id="5a0f4-114">String</span></span>                    |<span data-ttu-id="5a0f4-115">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="5a0f4-115">Parameter name.</span></span> |
|<span data-ttu-id="5a0f4-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="5a0f4-116">required</span></span>                    |<span data-ttu-id="5a0f4-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a0f4-117">Boolean</span></span>                   |<span data-ttu-id="5a0f4-118">`true` значение, если параметр является обязательным; в противном случае `false` .</span><span class="sxs-lookup"><span data-stu-id="5a0f4-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="5a0f4-119">type</span><span class="sxs-lookup"><span data-stu-id="5a0f4-119">type</span></span>                        |<span data-ttu-id="5a0f4-120">String</span><span class="sxs-lookup"><span data-stu-id="5a0f4-120">String</span></span>                    |<span data-ttu-id="5a0f4-121">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="5a0f4-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="5a0f4-122">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="5a0f4-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a0f4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a0f4-123">JSON representation</span></span>

<span data-ttu-id="5a0f4-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a0f4-124">The following is a JSON representation of the resource.</span></span>

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


