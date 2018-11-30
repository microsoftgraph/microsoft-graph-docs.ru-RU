---
title: Тип ресурса attributeMappingParameterSchema
description: Описывает один параметр, используемый в attributeMappingFunctionSchema.
ms.openlocfilehash: 164387a345f245f390d24b89a349e02ee2242041
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081506"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="38ca6-103">Тип ресурса attributeMappingParameterSchema</span><span class="sxs-lookup"><span data-stu-id="38ca6-103">attributeMappingParameterSchema resource type</span></span>

> <span data-ttu-id="38ca6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38ca6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38ca6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38ca6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38ca6-106">Описывает один параметр, используемый в [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span><span class="sxs-lookup"><span data-stu-id="38ca6-106">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="38ca6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="38ca6-107">Properties</span></span>

| <span data-ttu-id="38ca6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="38ca6-108">Property</span></span>                   | <span data-ttu-id="38ca6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="38ca6-109">Type</span></span>                      | <span data-ttu-id="38ca6-110">Description</span><span class="sxs-lookup"><span data-stu-id="38ca6-110">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="38ca6-111">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="38ca6-111">allowMultipleOccurrences</span></span>    |<span data-ttu-id="38ca6-112">Логический</span><span class="sxs-lookup"><span data-stu-id="38ca6-112">Boolean</span></span>                   |<span data-ttu-id="38ca6-113">Данному параметру можно указать несколько раз (например нескольких входных данных строки в `Concatenate(string,string,...)` функция).</span><span class="sxs-lookup"><span data-stu-id="38ca6-113">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="38ca6-114">name</span><span class="sxs-lookup"><span data-stu-id="38ca6-114">name</span></span>                        |<span data-ttu-id="38ca6-115">String</span><span class="sxs-lookup"><span data-stu-id="38ca6-115">String</span></span>                    |<span data-ttu-id="38ca6-116">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="38ca6-116">Parameter name.</span></span> |
|<span data-ttu-id="38ca6-117">Обязательный</span><span class="sxs-lookup"><span data-stu-id="38ca6-117">required</span></span>                    |<span data-ttu-id="38ca6-118">Логический</span><span class="sxs-lookup"><span data-stu-id="38ca6-118">Boolean</span></span>                   |<span data-ttu-id="38ca6-119">`true`Если параметр является обязательным; в противном случае `false`.</span><span class="sxs-lookup"><span data-stu-id="38ca6-119">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="38ca6-120">type</span><span class="sxs-lookup"><span data-stu-id="38ca6-120">type</span></span>                        |<span data-ttu-id="38ca6-121">String</span><span class="sxs-lookup"><span data-stu-id="38ca6-121">String</span></span>                    |<span data-ttu-id="38ca6-122">Возможные значения: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span><span class="sxs-lookup"><span data-stu-id="38ca6-122">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="38ca6-123">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="38ca6-123">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38ca6-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38ca6-124">JSON representation</span></span>

<span data-ttu-id="38ca6-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38ca6-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->