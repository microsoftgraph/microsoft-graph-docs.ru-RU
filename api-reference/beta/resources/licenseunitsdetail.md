---
title: Тип ресурса licenseUnitsDetail
description: Свойство **prepaidUnits** объекта subscribedSku относится к типу **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: michaelcurnutt
ms.openlocfilehash: 0f2f069cbbff191cefcdc8b735b2847b48a8f2ed
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030784"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="a6ea8-103">Тип ресурса licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="a6ea8-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="a6ea8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6ea8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6ea8-105">Свойство **prepaidUnits** объекта [subscribedSku](subscribedsku.md) относится к типу **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="a6ea8-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span> <span data-ttu-id="a6ea8-106">Дополнительные сведения о состояниях прогрессии подписки см. в журнале [What if my subscription expires?](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="a6ea8-106">For more information on the progression states of a subscription, see [What if my subscription expires?](/microsoft-365/commerce/subscriptions/what-if-my-subscription-expires?view=o365-worldwide)</span></span>

## <a name="properties"></a><span data-ttu-id="a6ea8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6ea8-107">Properties</span></span>
| <span data-ttu-id="a6ea8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6ea8-108">Property</span></span>     | <span data-ttu-id="a6ea8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a6ea8-109">Type</span></span>   |<span data-ttu-id="a6ea8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a6ea8-110">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="a6ea8-111">enabled</span><span class="sxs-lookup"><span data-stu-id="a6ea8-111">enabled</span></span>|<span data-ttu-id="a6ea8-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a6ea8-112">Int32</span></span>| <span data-ttu-id="a6ea8-113">Количество единиц, включенных для активной подписки службы SKU.</span><span class="sxs-lookup"><span data-stu-id="a6ea8-113">The number of units that are enabled for the active subscription of the service SKU.</span></span> |
|<span data-ttu-id="a6ea8-114">suspended</span><span class="sxs-lookup"><span data-stu-id="a6ea8-114">suspended</span></span>|<span data-ttu-id="a6ea8-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a6ea8-115">Int32</span></span>| <span data-ttu-id="a6ea8-116">Количество единиц, которые приостановлены из-за отмены подписки на службу SKU.</span><span class="sxs-lookup"><span data-stu-id="a6ea8-116">The number of units that are suspended because the subscription of the service SKU has been cancelled.</span></span> <span data-ttu-id="a6ea8-117">Эти блоки не могут быть назначены, но могут быть повторно активированы перед удалением.</span><span class="sxs-lookup"><span data-stu-id="a6ea8-117">The units cannot be assigned but can still be reactivated before they are deleted.</span></span> |
|<span data-ttu-id="a6ea8-118">warning</span><span class="sxs-lookup"><span data-stu-id="a6ea8-118">warning</span></span>|<span data-ttu-id="a6ea8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a6ea8-119">Int32</span></span>| <span data-ttu-id="a6ea8-120">Количество единиц, которые находятся в состоянии предупреждения.</span><span class="sxs-lookup"><span data-stu-id="a6ea8-120">The number of units that are in warning status.</span></span> <span data-ttu-id="a6ea8-121">По истечении срока действия подписки на службу SKU у клиента есть льготный период для продления подписки до ее отмены (перенесенной в **приостановленное** состояние).</span><span class="sxs-lookup"><span data-stu-id="a6ea8-121">When the subscription of the service SKU has expired, the customer has a grace period to renew their subscription before it is cancelled (moved to a **suspended** state).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6ea8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6ea8-122">JSON representation</span></span>

<span data-ttu-id="a6ea8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6ea8-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


