---
title: Тип ресурса Планнерпланконтекстдетаилсколлектион
description: " значение — объект Планнерпланконтекстдетаилс."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ce1d59c96b70da1533e7199d8b39b89f08f729aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521687"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="e06cf-103">Тип ресурса Планнерпланконтекстдетаилсколлектион</span><span class="sxs-lookup"><span data-stu-id="e06cf-103">plannerPlanContextDetailsCollection resource type</span></span>

<span data-ttu-id="e06cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e06cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="e06cf-105">Ресурс **планнерпланконтекстдетаилсколлектион** представляет коллекцию внешних контекстов, с которыми связан план.</span><span class="sxs-lookup"><span data-stu-id="e06cf-105">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="e06cf-106">Этот ресурс является открытым типом и является частью объекта [plannerPlanDetails](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="e06cf-106">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="e06cf-107">Имя свойства в аргументе "свойство-значение" — это идентификатор контекста, зависящий от приложения; значение — объект [планнерпланконтекстдетаилс](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="e06cf-107">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="e06cf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e06cf-108">Properties</span></span>
<span data-ttu-id="e06cf-109">Клиентская возможность может определять свойства открытого типа.</span><span class="sxs-lookup"><span data-stu-id="e06cf-109">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="e06cf-110">В этом случае клиент должен использовать отличительный идентификатор, представляющий внешний контекст в качестве имени свойства.</span><span class="sxs-lookup"><span data-stu-id="e06cf-110">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="e06cf-111">Значения свойств должны быть [планнерпланконтекстдетаилс](plannerplancontextdetails.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="e06cf-111">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="e06cf-112">На основе OData имена свойств в открытых типах не могут содержать следующие символы `.`:, `:`, `@`,. `%`</span><span class="sxs-lookup"><span data-stu-id="e06cf-112">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="e06cf-113">Эти символы необходимо закодировать с помощью формата кодирования URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="e06cf-113">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="e06cf-114">Чтобы удалить элемент из списка "Избранное", необходимо удалить его из коллекции [планнерпланконтекстколлектион](plannerplancontextcollection.md) , что приведет к автоматическому удалению записи в этом объекте.</span><span class="sxs-lookup"><span data-stu-id="e06cf-114">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e06cf-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e06cf-115">JSON representation</span></span>
<span data-ttu-id="e06cf-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e06cf-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
}-->

```json
{
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
