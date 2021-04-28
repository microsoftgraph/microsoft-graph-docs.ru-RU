---
title: тип ресурса alterationResponse
description: Предоставляет сведения, связанные с исправлениями орфографии в ответе на изменения.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e23b94b4e35776b2278c7818efc71f14edcc6cbb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068236"
---
# <a name="alterationresponse-resource-type"></a><span data-ttu-id="b849b-103">тип ресурса alterationResponse</span><span class="sxs-lookup"><span data-stu-id="b849b-103">alterationResponse resource type</span></span>

<span data-ttu-id="b849b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b849b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b849b-105">Предоставляет сведения, связанные с исправлениями орфографии в ответе на изменения.</span><span class="sxs-lookup"><span data-stu-id="b849b-105">Provides information related to spelling corrections in the alteration response.</span></span>

## <a name="properties"></a><span data-ttu-id="b849b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b849b-106">Properties</span></span>

| <span data-ttu-id="b849b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b849b-107">Property</span></span>     | <span data-ttu-id="b849b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b849b-108">Type</span></span>        | <span data-ttu-id="b849b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b849b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b849b-110">originalQueryString</span><span class="sxs-lookup"><span data-stu-id="b849b-110">originalQueryString</span></span>|<span data-ttu-id="b849b-111">String</span><span class="sxs-lookup"><span data-stu-id="b849b-111">String</span></span>| <span data-ttu-id="b849b-112">Определяет исходную строку запроса пользователя.</span><span class="sxs-lookup"><span data-stu-id="b849b-112">Defines the original user query string.</span></span>|
|<span data-ttu-id="b849b-113">queryAlteration</span><span class="sxs-lookup"><span data-stu-id="b849b-113">queryAlteration</span></span>|[<span data-ttu-id="b849b-114">searchAlteration</span><span class="sxs-lookup"><span data-stu-id="b849b-114">searchAlteration</span></span>](searchalteration.md)| <span data-ttu-id="b849b-115">Определяет сведения об изменениях для исправления орфографии.</span><span class="sxs-lookup"><span data-stu-id="b849b-115">Defines the details of alteration information for the spelling correction.</span></span>|
|<span data-ttu-id="b849b-116">queryAlterationType</span><span class="sxs-lookup"><span data-stu-id="b849b-116">queryAlterationType</span></span>|<span data-ttu-id="b849b-117">searchAlterationType</span><span class="sxs-lookup"><span data-stu-id="b849b-117">searchAlterationType</span></span>| <span data-ttu-id="b849b-118">Определяет тип коррекции орфографии.</span><span class="sxs-lookup"><span data-stu-id="b849b-118">Defines the type of the spelling correction.</span></span> <span data-ttu-id="b849b-119">Возможные значения `suggestion` : `modification` .</span><span class="sxs-lookup"><span data-stu-id="b849b-119">Possible values are `suggestion`, `modification`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b849b-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b849b-120">JSON representation</span></span>

<span data-ttu-id="b849b-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b849b-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alterationResponse",
  "baseType": null
}-->

```json
{
  "originalQueryString": "String",
  "queryAlteration": "String",
  "queryAlterationType": "suggestion"
}
```
