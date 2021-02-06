---
title: Тип ресурса attributeMappingParameterSchema
description: Описывает один параметр, используемый в атрибутеMappingFunctionSchema.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c8779211382ffcf7284c5ebf4035be6134efd8bf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128738"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="04adf-103">Тип ресурса attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="04adf-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="04adf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04adf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04adf-105">Описывает один параметр, используемый в [атрибутеMappingFunctionSchema.](../resources/synchronization-attributemappingfunctionschema.md)</span><span class="sxs-lookup"><span data-stu-id="04adf-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="04adf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="04adf-106">Properties</span></span>

| <span data-ttu-id="04adf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="04adf-107">Property</span></span>                   | <span data-ttu-id="04adf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="04adf-108">Type</span></span>                      | <span data-ttu-id="04adf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="04adf-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="04adf-110">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="04adf-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="04adf-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="04adf-111">Boolean</span></span>                   |<span data-ttu-id="04adf-112">Заданный параметр может быть предоставлен несколько раз (например, несколько строк ввода в `Concatenate(string,string,...)` функции).</span><span class="sxs-lookup"><span data-stu-id="04adf-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="04adf-113">name</span><span class="sxs-lookup"><span data-stu-id="04adf-113">name</span></span>                        |<span data-ttu-id="04adf-114">String</span><span class="sxs-lookup"><span data-stu-id="04adf-114">String</span></span>                    |<span data-ttu-id="04adf-115">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="04adf-115">Parameter name.</span></span> |
|<span data-ttu-id="04adf-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="04adf-116">required</span></span>                    |<span data-ttu-id="04adf-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="04adf-117">Boolean</span></span>                   |<span data-ttu-id="04adf-118">`true` если параметр является требуемой; в противном `false` случае .</span><span class="sxs-lookup"><span data-stu-id="04adf-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="04adf-119">type</span><span class="sxs-lookup"><span data-stu-id="04adf-119">type</span></span>                        |<span data-ttu-id="04adf-120">Строка</span><span class="sxs-lookup"><span data-stu-id="04adf-120">String</span></span>                    |<span data-ttu-id="04adf-121">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="04adf-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="04adf-122">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="04adf-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04adf-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04adf-123">JSON representation</span></span>

<span data-ttu-id="04adf-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04adf-124">The following is a JSON representation of the resource.</span></span>

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


