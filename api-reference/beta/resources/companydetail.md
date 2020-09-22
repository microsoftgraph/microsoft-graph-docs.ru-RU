---
title: Тип ресурса Компанидетаил
description: Тип ресурса Компанидетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 93b5490048c149ca526a9c3d0024175c1c20d7e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033932"
---
# <a name="companydetail-resource-type"></a><span data-ttu-id="490d1-103">Тип ресурса Компанидетаил</span><span class="sxs-lookup"><span data-stu-id="490d1-103">companyDetail resource type</span></span>

<span data-ttu-id="490d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="490d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="490d1-105">Представляет сведения о компаниях, связанных с сущностями в своем [профиле](profile.md).</span><span class="sxs-lookup"><span data-stu-id="490d1-105">Represents information about companies related to entities within their [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="490d1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="490d1-106">Properties</span></span>

| <span data-ttu-id="490d1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="490d1-107">Property</span></span>       | <span data-ttu-id="490d1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="490d1-108">Type</span></span>                                | <span data-ttu-id="490d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="490d1-109">Description</span></span>                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|<span data-ttu-id="490d1-110">address</span><span class="sxs-lookup"><span data-stu-id="490d1-110">address</span></span>         |[<span data-ttu-id="490d1-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="490d1-111">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="490d1-112">Адрес компании.</span><span class="sxs-lookup"><span data-stu-id="490d1-112">Address of the company.</span></span>                     |
|<span data-ttu-id="490d1-113">department</span><span class="sxs-lookup"><span data-stu-id="490d1-113">department</span></span>      |<span data-ttu-id="490d1-114">String</span><span class="sxs-lookup"><span data-stu-id="490d1-114">String</span></span>                               | <span data-ttu-id="490d1-115">Название отдела в компании.</span><span class="sxs-lookup"><span data-stu-id="490d1-115">Department Name within a company.</span></span>           |
|<span data-ttu-id="490d1-116">displayName</span><span class="sxs-lookup"><span data-stu-id="490d1-116">displayName</span></span>     |<span data-ttu-id="490d1-117">String</span><span class="sxs-lookup"><span data-stu-id="490d1-117">String</span></span>                               | <span data-ttu-id="490d1-118">Название компании.</span><span class="sxs-lookup"><span data-stu-id="490d1-118">Company name.</span></span>                               |
|<span data-ttu-id="490d1-119">officeLocation</span><span class="sxs-lookup"><span data-stu-id="490d1-119">officeLocation</span></span>  |<span data-ttu-id="490d1-120">String</span><span class="sxs-lookup"><span data-stu-id="490d1-120">String</span></span>                               | <span data-ttu-id="490d1-121">Местонахождение комнаты для пользователя, на который ссылается.</span><span class="sxs-lookup"><span data-stu-id="490d1-121">Office Location of the person referred to.</span></span>  |
|<span data-ttu-id="490d1-122">произношение</span><span class="sxs-lookup"><span data-stu-id="490d1-122">pronunciation</span></span>   |<span data-ttu-id="490d1-123">String</span><span class="sxs-lookup"><span data-stu-id="490d1-123">String</span></span>                               | <span data-ttu-id="490d1-124">Рекомендации по произношению названия компании.</span><span class="sxs-lookup"><span data-stu-id="490d1-124">Pronunciation guide for the company name.</span></span>   |
|<span data-ttu-id="490d1-125">webUrl</span><span class="sxs-lookup"><span data-stu-id="490d1-125">webUrl</span></span>          |<span data-ttu-id="490d1-126">String</span><span class="sxs-lookup"><span data-stu-id="490d1-126">String</span></span>                               | <span data-ttu-id="490d1-127">Ссылка на домашнюю страницу компании.</span><span class="sxs-lookup"><span data-stu-id="490d1-127">Link to the company home page.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="490d1-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="490d1-128">JSON representation</span></span>

<span data-ttu-id="490d1-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="490d1-129">The following is a JSON representation of the resource.</span></span>

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

