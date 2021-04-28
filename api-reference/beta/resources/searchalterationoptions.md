---
title: тип ресурса searchAlterationOptions
description: Предоставляет параметры изменения поиска для коррекции правописания.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: dc17698715b4ea6e894ae13f1999e78ab361cc5e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068245"
---
# <a name="searchalterationoptions-resource-type"></a><span data-ttu-id="11d9e-103">тип ресурса searchAlterationOptions</span><span class="sxs-lookup"><span data-stu-id="11d9e-103">searchAlterationOptions resource type</span></span>

<span data-ttu-id="11d9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11d9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11d9e-105">Предоставляет параметры изменения поиска для коррекции правописания.</span><span class="sxs-lookup"><span data-stu-id="11d9e-105">Provides the search alteration options for spelling correction.</span></span>

## <a name="properties"></a><span data-ttu-id="11d9e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="11d9e-106">Properties</span></span>

| <span data-ttu-id="11d9e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="11d9e-107">Property</span></span>     | <span data-ttu-id="11d9e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="11d9e-108">Type</span></span>        | <span data-ttu-id="11d9e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="11d9e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11d9e-110">enableSuggestion</span><span class="sxs-lookup"><span data-stu-id="11d9e-110">enableSuggestion</span></span>|<span data-ttu-id="11d9e-111">Логический</span><span class="sxs-lookup"><span data-stu-id="11d9e-111">Boolean</span></span>|<span data-ttu-id="11d9e-112">Указывает, включены ли предложения орфографии.</span><span class="sxs-lookup"><span data-stu-id="11d9e-112">Indicates whether spelling suggestions are enabled.</span></span> <span data-ttu-id="11d9e-113">Если включен, пользователь получит результаты поиска для исходного запроса поиска и предложит исправление [](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) орфографии в **свойстве queryAlterationResponse** ответа на опечатки в запросе.</span><span class="sxs-lookup"><span data-stu-id="11d9e-113">If enabled, user will get the search results for original search query and suggesting spelling correction in **queryAlterationResponse** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) for typos in query.</span></span> <span data-ttu-id="11d9e-114">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="11d9e-114">Optional.</span></span>|
|<span data-ttu-id="11d9e-115">enableModification</span><span class="sxs-lookup"><span data-stu-id="11d9e-115">enableModification</span></span>|<span data-ttu-id="11d9e-116">Логический</span><span class="sxs-lookup"><span data-stu-id="11d9e-116">Boolean</span></span>|<span data-ttu-id="11d9e-117">Указывает, включены ли изменения орфографии.</span><span class="sxs-lookup"><span data-stu-id="11d9e-117">Indicates whether spelling modifications are enabled.</span></span> <span data-ttu-id="11d9e-118">Если включен, пользователь получит результаты поиска  для исправленного запроса, если нет результатов для исходного запроса с опечатки и получит сведения о внесении изменений орфографии в **свойство queryAlterationResponse** ответа [.](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="11d9e-118">If enabled, user will get the search results for corrected query **when there are no results** for the original query with typos and get the spelling modification information in **queryAlterationResponse** property of the [response](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="11d9e-119">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="11d9e-119">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11d9e-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="11d9e-120">JSON representation</span></span>

<span data-ttu-id="11d9e-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11d9e-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlterationOptions",
  "baseType": null
}-->

```json
{
  "enableSuggestion": true,
  "enableModification": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchAlterationOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
