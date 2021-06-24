---
title: тип ресурса activateService
description: Представляет службу, которая должна быть активирована.
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a1ab2112406d0049df002327be784c46b7e879e6
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109193"
---
# <a name="activateservice-resource-type"></a><span data-ttu-id="84ded-103">тип ресурса activateService</span><span class="sxs-lookup"><span data-stu-id="84ded-103">activateService resource type</span></span>

<span data-ttu-id="84ded-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84ded-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84ded-105">Представляет службу, которая должна быть активирована.</span><span class="sxs-lookup"><span data-stu-id="84ded-105">Represents a service to be activated.</span></span>

## <a name="properties"></a><span data-ttu-id="84ded-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="84ded-106">Properties</span></span>

| <span data-ttu-id="84ded-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="84ded-107">Property</span></span>         | <span data-ttu-id="84ded-108">Тип</span><span class="sxs-lookup"><span data-stu-id="84ded-108">Type</span></span>         | <span data-ttu-id="84ded-109">Описание</span><span class="sxs-lookup"><span data-stu-id="84ded-109">Description</span></span>                           |
| ----------------- | ------------ | ------------------------------------- |
| <span data-ttu-id="84ded-110">service</span><span class="sxs-lookup"><span data-stu-id="84ded-110">service</span></span>| <span data-ttu-id="84ded-111">String</span><span class="sxs-lookup"><span data-stu-id="84ded-111">String</span></span> | <span data-ttu-id="84ded-112">Имя службы для активации.</span><span class="sxs-lookup"><span data-stu-id="84ded-112">The name of the service to activate.</span></span> |
| <span data-ttu-id="84ded-113">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="84ded-113">servicePlanId</span></span> | <span data-ttu-id="84ded-114">GUID</span><span class="sxs-lookup"><span data-stu-id="84ded-114">GUID</span></span> | <span data-ttu-id="84ded-115">Идентификатор плана для активации плана службы.</span><span class="sxs-lookup"><span data-stu-id="84ded-115">The plan identifier of the service plan to activate.</span></span> |
| <span data-ttu-id="84ded-116">skuId</span><span class="sxs-lookup"><span data-stu-id="84ded-116">skuId</span></span> | <span data-ttu-id="84ded-117">GUID</span><span class="sxs-lookup"><span data-stu-id="84ded-117">GUID</span></span> | <span data-ttu-id="84ded-118">Идентификатор SKU плана службы.</span><span class="sxs-lookup"><span data-stu-id="84ded-118">The SKU identifier of the service plan.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84ded-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84ded-119">JSON representation</span></span>

<span data-ttu-id="84ded-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84ded-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activateService"
}-->

```json
{
    "service": "string",
    "skuId": "guid",
    "servicePlanId": "guid"
}

```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activateService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
