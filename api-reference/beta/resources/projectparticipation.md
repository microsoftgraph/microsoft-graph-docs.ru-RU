---
title: Тип ресурса ПрожектпартиЦипатион
description: Тип ресурса ПрожектпартиЦипатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 465a45a2ba8a607d0537e66b96207b3d60626517
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950474"
---
# <a name="projectparticipation-resource-type"></a><span data-ttu-id="4ca02-103">Тип ресурса ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="4ca02-103">projectParticipation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ca02-104">Представляет подробные сведения о проектах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="4ca02-104">Represents detailed information about projects associated with a user.</span></span>

<span data-ttu-id="4ca02-105">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4ca02-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4ca02-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4ca02-106">Methods</span></span>

| <span data-ttu-id="4ca02-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4ca02-107">Method</span></span>                                                         | <span data-ttu-id="4ca02-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ca02-108">Return Type</span></span>                                     | <span data-ttu-id="4ca02-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4ca02-109">Description</span></span>                                                       |
|:---------------------------------------------------------------|:------------------------------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="4ca02-110">Получение ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="4ca02-110">Get projectParticipation</span></span>](../api/projectparticipation-get.md) | [<span data-ttu-id="4ca02-111">прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="4ca02-111">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="4ca02-112">Чтение свойств и связей объекта **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="4ca02-112">Read the properties and relationships of a **projectParticipation** object.</span></span> |
| [<span data-ttu-id="4ca02-113">Обновление ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="4ca02-113">Update projectParticipation</span></span>](../api/projectparticipation-update.md)                | [<span data-ttu-id="4ca02-114">прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="4ca02-114">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="4ca02-115">Обновление объекта **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="4ca02-115">Update a **projectParticipation** object.</span></span>                               |
| [<span data-ttu-id="4ca02-116">Удаление ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="4ca02-116">Delete projectParticipation</span></span>](../api/projectparticipation-delete.md)                | <span data-ttu-id="4ca02-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ca02-117">None.</span></span>                                            | <span data-ttu-id="4ca02-118">Удаление объекта **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="4ca02-118">Delete a **projectParticipation** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="4ca02-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ca02-119">Properties</span></span>

| <span data-ttu-id="4ca02-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ca02-120">Property</span></span>     | <span data-ttu-id="4ca02-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4ca02-121">Type</span></span>                                        | <span data-ttu-id="4ca02-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4ca02-122">Description</span></span>                                                                                      |
|:-------------|:--------------------------------------------|:-------------------------------------------------------------------------------------------------|
|<span data-ttu-id="4ca02-123">categories</span><span class="sxs-lookup"><span data-stu-id="4ca02-123">categories</span></span>    | <span data-ttu-id="4ca02-124">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4ca02-124">String collection</span></span>                           | <span data-ttu-id="4ca02-125">Содержит категории, связанные с проектом пользователем (например, цифровое преобразование, гидростенд).</span><span class="sxs-lookup"><span data-stu-id="4ca02-125">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="4ca02-126">Клиенты</span><span class="sxs-lookup"><span data-stu-id="4ca02-126">client</span></span>        |[<span data-ttu-id="4ca02-127">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="4ca02-127">companyDetail</span></span>](companydetail.md)            | <span data-ttu-id="4ca02-128">Содержит подробные сведения о клиенте, для которого выполнялся проект.</span><span class="sxs-lookup"><span data-stu-id="4ca02-128">Contains detailed information about the client the project was for.</span></span>                              |
|<span data-ttu-id="4ca02-129">коллег</span><span class="sxs-lookup"><span data-stu-id="4ca02-129">colleagues</span></span>    |<span data-ttu-id="4ca02-130">Коллекция [релатедперсон](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="4ca02-130">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="4ca02-131">Список людей, которые также работали над проектом.</span><span class="sxs-lookup"><span data-stu-id="4ca02-131">Lists people that also worked on the project.</span></span>                                                          |
|<span data-ttu-id="4ca02-132">описаны</span><span class="sxs-lookup"><span data-stu-id="4ca02-132">detail</span></span>        |[<span data-ttu-id="4ca02-133">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="4ca02-133">positionDetail</span></span>](positiondetail.md)          | <span data-ttu-id="4ca02-134">Содержит подробные сведения о роли пользователя в проекте.</span><span class="sxs-lookup"><span data-stu-id="4ca02-134">Contains detail about the user's role on the project.</span></span>                                             |
|<span data-ttu-id="4ca02-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4ca02-135">displayName</span></span>   |<span data-ttu-id="4ca02-136">String</span><span class="sxs-lookup"><span data-stu-id="4ca02-136">String</span></span>                                       |<span data-ttu-id="4ca02-137">Содержит понятное имя проекта.</span><span class="sxs-lookup"><span data-stu-id="4ca02-137">Contains a friendly name for the project.</span></span>                                                         |
|<span data-ttu-id="4ca02-138">спонсорами</span><span class="sxs-lookup"><span data-stu-id="4ca02-138">sponsors</span></span>      |<span data-ttu-id="4ca02-139">Коллекция [релатедперсон](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="4ca02-139">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="4ca02-140">Пользователь или люди, которые спонсорируют проект.</span><span class="sxs-lookup"><span data-stu-id="4ca02-140">The Person or people who sponsored the project.</span></span>                                                         |

## <a name="relationships"></a><span data-ttu-id="4ca02-141">Связи</span><span class="sxs-lookup"><span data-stu-id="4ca02-141">Relationships</span></span>

<span data-ttu-id="4ca02-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4ca02-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ca02-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ca02-143">JSON representation</span></span>

<span data-ttu-id="4ca02-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ca02-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.projectParticipation",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "client": {"@odata.type": "microsoft.graph.companyDetail"},
  "colleagues": [{"@odata.type": "microsoft.graph.relatedPerson"}],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"},
  "displayName": "String",
  "sponsors": [{"@odata.type": "microsoft.graph.relatedPerson"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "projectParticipation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
