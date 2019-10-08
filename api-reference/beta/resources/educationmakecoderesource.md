---
title: Тип ресурса Едукатионмакекодересаурце
description: Ресурс Макекоде
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5ffab7e11675996e79aed746cfe4624b28e37aab
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418288"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="8cbe2-103">Тип ресурса Едукатионмакекодересаурце</span><span class="sxs-lookup"><span data-stu-id="8cbe2-103">educationMakeCodeResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cbe2-104">Ресурс, представляющий проект [макекоде](https://www.microsoft.com/en-us/makecode) .</span><span class="sxs-lookup"><span data-stu-id="8cbe2-104">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="8cbe2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cbe2-105">Properties</span></span>

| <span data-ttu-id="8cbe2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cbe2-106">Property</span></span>     | <span data-ttu-id="8cbe2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8cbe2-107">Type</span></span>        | <span data-ttu-id="8cbe2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8cbe2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cbe2-109">projectId</span><span class="sxs-lookup"><span data-stu-id="8cbe2-109">projectId</span></span>|<span data-ttu-id="8cbe2-110">String</span><span class="sxs-lookup"><span data-stu-id="8cbe2-110">String</span></span>|<span data-ttu-id="8cbe2-111">ИДЕНТИФИКАТОР проекта Макекоде</span><span class="sxs-lookup"><span data-stu-id="8cbe2-111">ID of the MakeCode project</span></span>|
|<span data-ttu-id="8cbe2-112">хоствебурл</span><span class="sxs-lookup"><span data-stu-id="8cbe2-112">hostWebUrl</span></span>|<span data-ttu-id="8cbe2-113">String</span><span class="sxs-lookup"><span data-stu-id="8cbe2-113">String</span></span>|<span data-ttu-id="8cbe2-114">Узел для типа ресурса Макекоде (например, аркаде, Микробит)</span><span class="sxs-lookup"><span data-stu-id="8cbe2-114">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cbe2-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cbe2-115">JSON representation</span></span>

<span data-ttu-id="8cbe2-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cbe2-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "projectId": "String",
  "hostWebUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->