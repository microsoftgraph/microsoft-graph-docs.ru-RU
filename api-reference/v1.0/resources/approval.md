---
title: Тип ресурса утверждения
description: Объект утверждения, связанный с userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c6d41146551586f681ebf5ed7fda735151f1efc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469666"
---
# <a name="approval-resource-type"></a><span data-ttu-id="4824c-103">Тип ресурса утверждения</span><span class="sxs-lookup"><span data-stu-id="4824c-103">approval resource type</span></span>

<span data-ttu-id="4824c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4824c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4824c-105">Представляет объект утверждения для решений, связанных с запросом.</span><span class="sxs-lookup"><span data-stu-id="4824c-105">Represents the approval object for decisions associated with a request.</span></span>

## <a name="properties"></a><span data-ttu-id="4824c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4824c-106">Properties</span></span>

|<span data-ttu-id="4824c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4824c-107">Property</span></span>|<span data-ttu-id="4824c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4824c-108">Type</span></span>|<span data-ttu-id="4824c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4824c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4824c-110">id</span><span class="sxs-lookup"><span data-stu-id="4824c-110">id</span></span>|<span data-ttu-id="4824c-111">String</span><span class="sxs-lookup"><span data-stu-id="4824c-111">String</span></span>|<span data-ttu-id="4824c-112">Идентификатор решения об утверждении.</span><span class="sxs-lookup"><span data-stu-id="4824c-112">Identifier of the approval decision.</span></span>|
|<span data-ttu-id="4824c-113">stages</span><span class="sxs-lookup"><span data-stu-id="4824c-113">stages</span></span>|<span data-ttu-id="4824c-114">[коллекция approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="4824c-114">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="4824c-115">Набор этапов в решении об утверждении.</span><span class="sxs-lookup"><span data-stu-id="4824c-115">A collection of stages in the approval decision.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4824c-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4824c-116">Relationships</span></span>

|<span data-ttu-id="4824c-117">Связь</span><span class="sxs-lookup"><span data-stu-id="4824c-117">Relationship</span></span>|<span data-ttu-id="4824c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="4824c-118">Type</span></span>|<span data-ttu-id="4824c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4824c-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4824c-120">stages</span><span class="sxs-lookup"><span data-stu-id="4824c-120">stages</span></span>|<span data-ttu-id="4824c-121">[коллекция approvalStage](../resources/approvalstage.md)</span><span class="sxs-lookup"><span data-stu-id="4824c-121">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="4824c-122">Набор этапов в решении об утверждении.</span><span class="sxs-lookup"><span data-stu-id="4824c-122">A collection of stages in the approval decision.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4824c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4824c-123">JSON representation</span></span>

<span data-ttu-id="4824c-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4824c-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "stages": [{
        "@odata.type": "#microsoft.graph.approvalStage"
    }]
}
```
