---
title: Тип ресурса Компанидетаил
description: Тип ресурса Компанидетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 04e33c9fdae1eae811ee88e7cdef95b4b97b2c3f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936841"
---
# <a name="companydetail-resource-type"></a><span data-ttu-id="f6db5-103">Тип ресурса Компанидетаил</span><span class="sxs-lookup"><span data-stu-id="f6db5-103">companyDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6db5-104">Представляет сведения о компаниях, связанных с сущностями в своем [профиле](profile.md).</span><span class="sxs-lookup"><span data-stu-id="f6db5-104">Represents information about companies related to entities within their [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f6db5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6db5-105">Properties</span></span>

| <span data-ttu-id="f6db5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6db5-106">Property</span></span>       | <span data-ttu-id="f6db5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f6db5-107">Type</span></span>                                | <span data-ttu-id="f6db5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f6db5-108">Description</span></span>                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|<span data-ttu-id="f6db5-109">address</span><span class="sxs-lookup"><span data-stu-id="f6db5-109">address</span></span>         |[<span data-ttu-id="f6db5-110">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f6db5-110">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="f6db5-111">Адрес компании.</span><span class="sxs-lookup"><span data-stu-id="f6db5-111">Address of the company.</span></span>                     |
|<span data-ttu-id="f6db5-112">department</span><span class="sxs-lookup"><span data-stu-id="f6db5-112">department</span></span>      |<span data-ttu-id="f6db5-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f6db5-113">String</span></span>                               | <span data-ttu-id="f6db5-114">Название отдела в компании.</span><span class="sxs-lookup"><span data-stu-id="f6db5-114">Department Name within a company.</span></span>           |
|<span data-ttu-id="f6db5-115">displayName</span><span class="sxs-lookup"><span data-stu-id="f6db5-115">displayName</span></span>     |<span data-ttu-id="f6db5-116">Строка</span><span class="sxs-lookup"><span data-stu-id="f6db5-116">String</span></span>                               | <span data-ttu-id="f6db5-117">Название компании.</span><span class="sxs-lookup"><span data-stu-id="f6db5-117">Company name.</span></span>                               |
|<span data-ttu-id="f6db5-118">officeLocation</span><span class="sxs-lookup"><span data-stu-id="f6db5-118">officeLocation</span></span>  |<span data-ttu-id="f6db5-119">String</span><span class="sxs-lookup"><span data-stu-id="f6db5-119">String</span></span>                               | <span data-ttu-id="f6db5-120">Местонахождение комнаты для пользователя, на который ссылается.</span><span class="sxs-lookup"><span data-stu-id="f6db5-120">Office Location of the person referred to.</span></span>  |
|<span data-ttu-id="f6db5-121">произношение</span><span class="sxs-lookup"><span data-stu-id="f6db5-121">pronunciation</span></span>   |<span data-ttu-id="f6db5-122">Строка</span><span class="sxs-lookup"><span data-stu-id="f6db5-122">String</span></span>                               | <span data-ttu-id="f6db5-123">Рекомендации по произношению названия компании.</span><span class="sxs-lookup"><span data-stu-id="f6db5-123">Pronunciation guide for the company name.</span></span>   |
|<span data-ttu-id="f6db5-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="f6db5-124">webUrl</span></span>          |<span data-ttu-id="f6db5-125">String</span><span class="sxs-lookup"><span data-stu-id="f6db5-125">String</span></span>                               | <span data-ttu-id="f6db5-126">Ссылка на домашнюю страницу компании.</span><span class="sxs-lookup"><span data-stu-id="f6db5-126">Link to the company home page.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="f6db5-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6db5-127">JSON representation</span></span>

<span data-ttu-id="f6db5-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6db5-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.companyDetail",
  "baseType": null
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "department": "String",
  "displayName": "String",
  "officeLocation": "String",
  "pronunciation": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "companyDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->