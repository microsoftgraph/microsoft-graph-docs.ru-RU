---
title: Тип ресурса plannerPlanContextDetailsCollection
description: " значение — это объект plannerPlanContextDetails."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: ca1625a4bf137fc14cc780df4d4d1e5ec3bb226e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642942"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="9e2ce-103">Тип ресурса plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="9e2ce-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="9e2ce-104">Ресурс **plannerPlanContextDetailsCollection** представляет коллекцию внешних контекстах, с которыми связан плана.</span><span class="sxs-lookup"><span data-stu-id="9e2ce-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="9e2ce-105">Этот ресурс является открытым и является частью объекта [plannerPlanDetails](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="9e2ce-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="9e2ce-106">Имя свойства в паре значение свойства — это идентификатор приложения определенного контекста; значение — это объект [plannerPlanContextDetails](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="9e2ce-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="9e2ce-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e2ce-107">Properties</span></span>
<span data-ttu-id="9e2ce-108">Свойства открытого типа может быть определен клиентом.</span><span class="sxs-lookup"><span data-stu-id="9e2ce-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="9e2ce-109">В этом случае клиент должен использовать особый идентификатор, представляющий внешнего контекста как имя свойства.</span><span class="sxs-lookup"><span data-stu-id="9e2ce-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="9e2ce-110">Значения свойства должны быть [plannerPlanContextDetails](plannerplancontextdetails.md) объектов.</span><span class="sxs-lookup"><span data-stu-id="9e2ce-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="9e2ce-111">На основании OData, имена свойств в открытые типы не может содержать следующие символы: `.`, `:`, `@`, `%`.</span><span class="sxs-lookup"><span data-stu-id="9e2ce-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="9e2ce-112">Эти символы должны кодируются с помощью кодировки формат URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="9e2ce-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="9e2ce-113">Удаление элемента из списка "Избранное", значение должно быть удален из коллекции [plannerPlanContextCollection](plannerplancontextcollection.md) вместо этого которого будет автоматически удалять запись в этот объект.</span><span class="sxs-lookup"><span data-stu-id="9e2ce-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetailscollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
