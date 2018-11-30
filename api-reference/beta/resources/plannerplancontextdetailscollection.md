---
title: Тип ресурса plannerPlanContextDetailsCollection
description: " значение — это объект plannerPlanContextDetails."
ms.openlocfilehash: 843be37ae0abc73de19e72c655b18834b7f5c03e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080242"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="e25f0-103">Тип ресурса plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="e25f0-103">plannerPlanContextDetailsCollection resource type</span></span>

> <span data-ttu-id="e25f0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e25f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e25f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e25f0-105">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="e25f0-106">Ресурс **plannerPlanContextDetailsCollection** представляет коллекцию внешних контекстах, с которыми связан плана.</span><span class="sxs-lookup"><span data-stu-id="e25f0-106">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="e25f0-107">Этот ресурс является открытым и является частью объекта [plannerPlanDetails](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="e25f0-107">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="e25f0-108">Имя свойства в паре значение свойства — это идентификатор приложения определенного контекста; значение — это объект [plannerPlanContextDetails](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="e25f0-108">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="e25f0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e25f0-109">Properties</span></span>
<span data-ttu-id="e25f0-110">Свойства открытого типа может быть определен клиентом.</span><span class="sxs-lookup"><span data-stu-id="e25f0-110">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="e25f0-111">В этом случае клиент должен использовать особый идентификатор, представляющий внешнего контекста как имя свойства.</span><span class="sxs-lookup"><span data-stu-id="e25f0-111">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="e25f0-112">Значения свойства должны быть [plannerPlanContextDetails](plannerplancontextdetails.md) объектов.</span><span class="sxs-lookup"><span data-stu-id="e25f0-112">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="e25f0-113">На основании OData, имена свойств в открытые типы не может содержать следующие символы: `.`, `:`, `@`, `%`.</span><span class="sxs-lookup"><span data-stu-id="e25f0-113">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="e25f0-114">Эти символы должны кодируются с помощью кодировки формат URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="e25f0-114">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="e25f0-115">Удаление элемента из списка "Избранное", значение должно быть удален из коллекции [plannerPlanContextCollection](plannerplancontextcollection.md) вместо этого которого будет автоматически удалять запись в этот объект.</span><span class="sxs-lookup"><span data-stu-id="e25f0-115">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
