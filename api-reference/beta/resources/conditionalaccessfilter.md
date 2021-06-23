---
title: тип ресурса conditionalAccessFilter
description: Представляет фильтр в области политики.
localization_priority: Normal
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f5b14a3faa593453c88cc155f7e44348fcfda35
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082410"
---
# <a name="conditionalaccessfilter-resource-type"></a><span data-ttu-id="500f6-103">тип ресурса conditionalAccessFilter</span><span class="sxs-lookup"><span data-stu-id="500f6-103">conditionalAccessFilter resource type</span></span>

<span data-ttu-id="500f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="500f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="500f6-105">Представляет фильтр в области политики.</span><span class="sxs-lookup"><span data-stu-id="500f6-105">Represents filter in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="500f6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="500f6-106">Properties</span></span>

| <span data-ttu-id="500f6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="500f6-107">Property</span></span>     | <span data-ttu-id="500f6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="500f6-108">Type</span></span>        | <span data-ttu-id="500f6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="500f6-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="500f6-110">mode</span><span class="sxs-lookup"><span data-stu-id="500f6-110">mode</span></span> | <span data-ttu-id="500f6-111">filterMode</span><span class="sxs-lookup"><span data-stu-id="500f6-111">filterMode</span></span> | <span data-ttu-id="500f6-112">Режим использования для фильтра.</span><span class="sxs-lookup"><span data-stu-id="500f6-112">Mode to use for the filter.</span></span> <span data-ttu-id="500f6-113">Возможные значения: `include` или `exclude`.</span><span class="sxs-lookup"><span data-stu-id="500f6-113">Possible values are `include` or `exclude`.</span></span> |
| <span data-ttu-id="500f6-114">правило</span><span class="sxs-lookup"><span data-stu-id="500f6-114">rule</span></span> | <span data-ttu-id="500f6-115">String</span><span class="sxs-lookup"><span data-stu-id="500f6-115">String</span></span> | <span data-ttu-id="500f6-116">Синтаксис правил похож на тот, который используется для правил членства для групп в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="500f6-116">Rule syntax is similar to that used for membership rules for groups in Azure AD.</span></span> <span data-ttu-id="500f6-117">Подробные сведения см. [в правилах с несколькими выражениями](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions)</span><span class="sxs-lookup"><span data-stu-id="500f6-117">For details, see [rules with multiple expressions](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions)</span></span> |

## <a name="relationships"></a><span data-ttu-id="500f6-118">Связи</span><span class="sxs-lookup"><span data-stu-id="500f6-118">Relationships</span></span>

<span data-ttu-id="500f6-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="500f6-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="500f6-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="500f6-120">JSON representation</span></span>

<span data-ttu-id="500f6-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="500f6-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "mode",
    "rule"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessFilter",
  "baseType": null
}-->

```json
{
  "mode": "String",
  "rule": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessFilter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


