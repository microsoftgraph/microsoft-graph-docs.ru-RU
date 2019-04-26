---
title: Тип ресурса Планнерпланконтекстдетаилсколлектион
description: " значение — объект Планнерпланконтекстдетаилс."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: ca1625a4bf137fc14cc780df4d4d1e5ec3bb226e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571859"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="215dc-103">Тип ресурса Планнерпланконтекстдетаилсколлектион</span><span class="sxs-lookup"><span data-stu-id="215dc-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="215dc-104">Ресурс **планнерпланконтекстдетаилсколлектион** представляет коллекцию внешних контекстов, с которыми связан план.</span><span class="sxs-lookup"><span data-stu-id="215dc-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="215dc-105">Этот ресурс является открытым типом и является частью объекта [plannerPlanDetails](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="215dc-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="215dc-106">Имя свойства в аргументе "свойство-значение" — это идентификатор контекста, зависящий от приложения; значение — объект [планнерпланконтекстдетаилс](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="215dc-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="215dc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="215dc-107">Properties</span></span>
<span data-ttu-id="215dc-108">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="215dc-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="215dc-109">В этом случае клиент должен использовать отличительный идентификатор, представляющий внешний контекст в качестве имени свойства.</span><span class="sxs-lookup"><span data-stu-id="215dc-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="215dc-110">Значения свойств должны быть [планнерпланконтекстдетаилс](plannerplancontextdetails.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="215dc-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="215dc-111">На основе OData имена свойств в открытых типах не могут содержать следующие символы `.`:, `:`, `@`,. `%`</span><span class="sxs-lookup"><span data-stu-id="215dc-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="215dc-112">Эти символы необходимо закодировать с помощью формата кодирования URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="215dc-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="215dc-113">Чтобы удалить элемент из списка "Избранное", необходимо удалить его из коллекции [планнерпланконтекстколлектион](plannerplancontextcollection.md) , что приведет к автоматическому удалению записи в этом объекте.</span><span class="sxs-lookup"><span data-stu-id="215dc-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


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
