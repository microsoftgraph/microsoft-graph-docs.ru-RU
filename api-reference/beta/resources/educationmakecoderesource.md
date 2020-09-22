---
title: Тип ресурса Едукатионмакекодересаурце
description: Ресурс Макекоде
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 49e0a563a190056159c8c910cc46398a6adee41d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076451"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="8f923-103">Тип ресурса Едукатионмакекодересаурце</span><span class="sxs-lookup"><span data-stu-id="8f923-103">educationMakeCodeResource resource type</span></span>

<span data-ttu-id="8f923-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f923-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f923-105">Ресурс, представляющий проект [макекоде](https://www.microsoft.com/en-us/makecode) .</span><span class="sxs-lookup"><span data-stu-id="8f923-105">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="8f923-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f923-106">Properties</span></span>

| <span data-ttu-id="8f923-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f923-107">Property</span></span>     | <span data-ttu-id="8f923-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8f923-108">Type</span></span>        | <span data-ttu-id="8f923-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8f923-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f923-110">projectId</span><span class="sxs-lookup"><span data-stu-id="8f923-110">projectId</span></span>|<span data-ttu-id="8f923-111">String</span><span class="sxs-lookup"><span data-stu-id="8f923-111">String</span></span>|<span data-ttu-id="8f923-112">ИДЕНТИФИКАТОР проекта Макекоде</span><span class="sxs-lookup"><span data-stu-id="8f923-112">ID of the MakeCode project</span></span>|
|<span data-ttu-id="8f923-113">хоствебурл</span><span class="sxs-lookup"><span data-stu-id="8f923-113">hostWebUrl</span></span>|<span data-ttu-id="8f923-114">String</span><span class="sxs-lookup"><span data-stu-id="8f923-114">String</span></span>|<span data-ttu-id="8f923-115">Узел для типа ресурса Макекоде (например, аркаде, Микробит)</span><span class="sxs-lookup"><span data-stu-id="8f923-115">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f923-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f923-116">JSON representation</span></span>

<span data-ttu-id="8f923-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f923-117">The following is a JSON representation of the resource.</span></span>

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

