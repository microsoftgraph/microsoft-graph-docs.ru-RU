---
title: Тип ресурса Компанидетаил
description: Тип ресурса Компанидетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dc8da38c9da8d6631e8e46199f420ae0b3ab652e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507585"
---
# <a name="companydetail-resource-type"></a><span data-ttu-id="5f2d6-103">Тип ресурса Компанидетаил</span><span class="sxs-lookup"><span data-stu-id="5f2d6-103">companyDetail resource type</span></span>

<span data-ttu-id="5f2d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f2d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f2d6-105">Представляет сведения о компаниях, связанных с сущностями в своем [профиле](profile.md).</span><span class="sxs-lookup"><span data-stu-id="5f2d6-105">Represents information about companies related to entities within their [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5f2d6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f2d6-106">Properties</span></span>

| <span data-ttu-id="5f2d6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f2d6-107">Property</span></span>       | <span data-ttu-id="5f2d6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5f2d6-108">Type</span></span>                                | <span data-ttu-id="5f2d6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5f2d6-109">Description</span></span>                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|<span data-ttu-id="5f2d6-110">address</span><span class="sxs-lookup"><span data-stu-id="5f2d6-110">address</span></span>         |[<span data-ttu-id="5f2d6-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5f2d6-111">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="5f2d6-112">Адрес компании.</span><span class="sxs-lookup"><span data-stu-id="5f2d6-112">Address of the company.</span></span>                     |
|<span data-ttu-id="5f2d6-113">отделу;</span><span class="sxs-lookup"><span data-stu-id="5f2d6-113">department</span></span>      |<span data-ttu-id="5f2d6-114">String</span><span class="sxs-lookup"><span data-stu-id="5f2d6-114">String</span></span>                               | <span data-ttu-id="5f2d6-115">Название отдела в компании.</span><span class="sxs-lookup"><span data-stu-id="5f2d6-115">Department Name within a company.</span></span>           |
|<span data-ttu-id="5f2d6-116">displayName</span><span class="sxs-lookup"><span data-stu-id="5f2d6-116">displayName</span></span>     |<span data-ttu-id="5f2d6-117">Строка</span><span class="sxs-lookup"><span data-stu-id="5f2d6-117">String</span></span>                               | <span data-ttu-id="5f2d6-118">Название компании.</span><span class="sxs-lookup"><span data-stu-id="5f2d6-118">Company name.</span></span>                               |
|<span data-ttu-id="5f2d6-119">officeLocation</span><span class="sxs-lookup"><span data-stu-id="5f2d6-119">officeLocation</span></span>  |<span data-ttu-id="5f2d6-120">String</span><span class="sxs-lookup"><span data-stu-id="5f2d6-120">String</span></span>                               | <span data-ttu-id="5f2d6-121">Местонахождение комнаты для пользователя, на который ссылается.</span><span class="sxs-lookup"><span data-stu-id="5f2d6-121">Office Location of the person referred to.</span></span>  |
|<span data-ttu-id="5f2d6-122">произношение</span><span class="sxs-lookup"><span data-stu-id="5f2d6-122">pronunciation</span></span>   |<span data-ttu-id="5f2d6-123">String</span><span class="sxs-lookup"><span data-stu-id="5f2d6-123">String</span></span>                               | <span data-ttu-id="5f2d6-124">Рекомендации по произношению названия компании.</span><span class="sxs-lookup"><span data-stu-id="5f2d6-124">Pronunciation guide for the company name.</span></span>   |
|<span data-ttu-id="5f2d6-125">webUrl</span><span class="sxs-lookup"><span data-stu-id="5f2d6-125">webUrl</span></span>          |<span data-ttu-id="5f2d6-126">String</span><span class="sxs-lookup"><span data-stu-id="5f2d6-126">String</span></span>                               | <span data-ttu-id="5f2d6-127">Ссылка на домашнюю страницу компании.</span><span class="sxs-lookup"><span data-stu-id="5f2d6-127">Link to the company home page.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="5f2d6-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f2d6-128">JSON representation</span></span>

<span data-ttu-id="5f2d6-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f2d6-129">The following is a JSON representation of the resource.</span></span>

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