---
title: тип ресурса resultTemplate
description: Словарь resultTemplateIds и связанных с ними значений, которые включают имя и схему JSON шаблонов результатов.
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 402b60efc278e72102d9bba4eb89be2dda38916b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211374"
---
# <a name="resulttemplate-resource-type"></a><span data-ttu-id="a84a1-103">тип ресурса resultTemplate</span><span class="sxs-lookup"><span data-stu-id="a84a1-103">resultTemplate resource type</span></span>

<span data-ttu-id="a84a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a84a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a84a1-105">Словарь **resultTemplateIds** и связанных значений, который включает имя и схему JSON шаблонов результатов.</span><span class="sxs-lookup"><span data-stu-id="a84a1-105">A dictionary of **resultTemplateIds** and associated values, which includes the name and JSON schema of the result templates.</span></span>

## <a name="properties"></a><span data-ttu-id="a84a1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a84a1-106">Properties</span></span>

| <span data-ttu-id="a84a1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a84a1-107">Property</span></span>     | <span data-ttu-id="a84a1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a84a1-108">Type</span></span>        | <span data-ttu-id="a84a1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a84a1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a84a1-110">key</span><span class="sxs-lookup"><span data-stu-id="a84a1-110">key</span></span>|<span data-ttu-id="a84a1-111">String</span><span class="sxs-lookup"><span data-stu-id="a84a1-111">String</span></span>|<span data-ttu-id="a84a1-112">ID шаблона результатов.</span><span class="sxs-lookup"><span data-stu-id="a84a1-112">ID of a result template.</span></span> <span data-ttu-id="a84a1-113">Он должен сопопозить **с resultTemplateId** в [searchHit.](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="a84a1-113">It must map to a **resultTemplateId** in the [searchHit](searchhit.md).</span></span>|
|<span data-ttu-id="a84a1-114">displayName</span><span class="sxs-lookup"><span data-stu-id="a84a1-114">displayName</span></span>|<span data-ttu-id="a84a1-115">String</span><span class="sxs-lookup"><span data-stu-id="a84a1-115">String</span></span>|<span data-ttu-id="a84a1-116">Имя шаблона результатов.</span><span class="sxs-lookup"><span data-stu-id="a84a1-116">Name of the result template.</span></span>|
|<span data-ttu-id="a84a1-117">body</span><span class="sxs-lookup"><span data-stu-id="a84a1-117">body</span></span>|<span data-ttu-id="a84a1-118">Json</span><span class="sxs-lookup"><span data-stu-id="a84a1-118">Json</span></span>|<span data-ttu-id="a84a1-119">Схема шаблона результатов JSON.</span><span class="sxs-lookup"><span data-stu-id="a84a1-119">JSON schema of the result template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a84a1-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a84a1-120">JSON representation</span></span>

<span data-ttu-id="a84a1-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a84a1-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplate",
  "baseType": null
}-->


```json
{
  "resultTemplateId": {
                    "displayName": "String",
                    "body": "Json schema"
                }
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


