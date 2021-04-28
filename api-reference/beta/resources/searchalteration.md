---
title: тип ресурса searchAlteration
description: Предоставляет сведения об изменениях поиска для исправления орфографии.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5caab3a3fbd8f8487e6893c5f5f530cc8471bb80
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068242"
---
# <a name="searchalteration-resource-type"></a><span data-ttu-id="b7362-103">тип ресурса searchAlteration</span><span class="sxs-lookup"><span data-stu-id="b7362-103">searchAlteration resource type</span></span>

<span data-ttu-id="b7362-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7362-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7362-105">Предоставляет сведения об изменениях поиска для исправления орфографии.</span><span class="sxs-lookup"><span data-stu-id="b7362-105">Provides the details of search alteration for spelling correction.</span></span>

## <a name="properties"></a><span data-ttu-id="b7362-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7362-106">Properties</span></span>

| <span data-ttu-id="b7362-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7362-107">Property</span></span>     | <span data-ttu-id="b7362-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b7362-108">Type</span></span>        | <span data-ttu-id="b7362-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b7362-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b7362-110">alteredQueryString</span><span class="sxs-lookup"><span data-stu-id="b7362-110">alteredQueryString</span></span>|<span data-ttu-id="b7362-111">String</span><span class="sxs-lookup"><span data-stu-id="b7362-111">String</span></span>| <span data-ttu-id="b7362-112">Определяет измененную строку запроса с помощью коррекции орфографии.</span><span class="sxs-lookup"><span data-stu-id="b7362-112">Defines the altered query string with spelling correction.</span></span>|
|<span data-ttu-id="b7362-113">alteredHighlightedQueryString</span><span class="sxs-lookup"><span data-stu-id="b7362-113">alteredHighlightedQueryString</span></span>|<span data-ttu-id="b7362-114">String</span><span class="sxs-lookup"><span data-stu-id="b7362-114">String</span></span>| <span data-ttu-id="b7362-115">Определяет измененную выделенную строку запроса с помощью коррекции орфографии.</span><span class="sxs-lookup"><span data-stu-id="b7362-115">Defines the altered highlighted query string with spelling correction.</span></span> <span data-ttu-id="b7362-116">Аннотация вокруг исправленного сегмента (\ue000, \ue001)</span><span class="sxs-lookup"><span data-stu-id="b7362-116">The annotation around the corrected segment is (\ue000, \ue001)</span></span>|
|<span data-ttu-id="b7362-117">alteredQueryTokens</span><span class="sxs-lookup"><span data-stu-id="b7362-117">alteredQueryTokens</span></span>|<span data-ttu-id="b7362-118">[измененная коллекцияQueryToken](alteredquerytoken.md)</span><span class="sxs-lookup"><span data-stu-id="b7362-118">[alteredQueryToken](alteredquerytoken.md) collection</span></span>| <span data-ttu-id="b7362-119">Представляет измененные сегменты в отношении исходного запроса.</span><span class="sxs-lookup"><span data-stu-id="b7362-119">Represents changed segments with respect to original query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7362-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b7362-120">JSON representation</span></span>

<span data-ttu-id="b7362-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7362-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlteration",
  "baseType": null
}-->

```json
{
  "alteredQueryString": "String",
  "alteredHighlightedQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```