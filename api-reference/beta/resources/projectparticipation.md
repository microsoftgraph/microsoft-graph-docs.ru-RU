---
title: Тип ресурса ПрожектпартиЦипатион
description: Тип ресурса ПрожектпартиЦипатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1aa9188f40175ba0f52f143081004d8c3cbc4797
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521434"
---
# <a name="projectparticipation-resource-type"></a><span data-ttu-id="ce553-103">Тип ресурса ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="ce553-103">projectParticipation resource type</span></span>

<span data-ttu-id="ce553-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ce553-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce553-105">Представляет подробные сведения о проектах, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="ce553-105">Represents detailed information about projects associated with a user.</span></span>

<span data-ttu-id="ce553-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ce553-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ce553-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ce553-107">Methods</span></span>

| <span data-ttu-id="ce553-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ce553-108">Method</span></span>                                                         | <span data-ttu-id="ce553-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce553-109">Return Type</span></span>                                     | <span data-ttu-id="ce553-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ce553-110">Description</span></span>                                                       |
|:---------------------------------------------------------------|:------------------------------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="ce553-111">Получение ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="ce553-111">Get projectParticipation</span></span>](../api/projectparticipation-get.md) | [<span data-ttu-id="ce553-112">прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="ce553-112">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="ce553-113">Чтение свойств и связей объекта **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="ce553-113">Read the properties and relationships of a **projectParticipation** object.</span></span> |
| [<span data-ttu-id="ce553-114">Обновление ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="ce553-114">Update projectParticipation</span></span>](../api/projectparticipation-update.md)                | [<span data-ttu-id="ce553-115">прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="ce553-115">projectParticipation</span></span>](projectparticipation.md) | <span data-ttu-id="ce553-116">Обновление объекта **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="ce553-116">Update a **projectParticipation** object.</span></span>                               |
| [<span data-ttu-id="ce553-117">Удаление ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="ce553-117">Delete projectParticipation</span></span>](../api/projectparticipation-delete.md)                | <span data-ttu-id="ce553-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="ce553-118">None.</span></span>                                            | <span data-ttu-id="ce553-119">Удаление объекта **прожектпартиЦипатион** .</span><span class="sxs-lookup"><span data-stu-id="ce553-119">Delete a **projectParticipation** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="ce553-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce553-120">Properties</span></span>

| <span data-ttu-id="ce553-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce553-121">Property</span></span>     | <span data-ttu-id="ce553-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ce553-122">Type</span></span>                                        | <span data-ttu-id="ce553-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ce553-123">Description</span></span>                                                                                      |
|:-------------|:--------------------------------------------|:-------------------------------------------------------------------------------------------------|
|<span data-ttu-id="ce553-124">categories</span><span class="sxs-lookup"><span data-stu-id="ce553-124">categories</span></span>    | <span data-ttu-id="ce553-125">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce553-125">String collection</span></span>                           | <span data-ttu-id="ce553-126">Содержит категории, связанные с проектом пользователем (например, цифровое преобразование, гидростенд).</span><span class="sxs-lookup"><span data-stu-id="ce553-126">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="ce553-127">Клиенты</span><span class="sxs-lookup"><span data-stu-id="ce553-127">client</span></span>        |[<span data-ttu-id="ce553-128">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="ce553-128">companyDetail</span></span>](companydetail.md)            | <span data-ttu-id="ce553-129">Содержит подробные сведения о клиенте, для которого выполнялся проект.</span><span class="sxs-lookup"><span data-stu-id="ce553-129">Contains detailed information about the client the project was for.</span></span>                              |
|<span data-ttu-id="ce553-130">коллег</span><span class="sxs-lookup"><span data-stu-id="ce553-130">colleagues</span></span>    |<span data-ttu-id="ce553-131">Коллекция [релатедперсон](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="ce553-131">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="ce553-132">Список людей, которые также работали над проектом.</span><span class="sxs-lookup"><span data-stu-id="ce553-132">Lists people that also worked on the project.</span></span>                                                          |
|<span data-ttu-id="ce553-133">описаны</span><span class="sxs-lookup"><span data-stu-id="ce553-133">detail</span></span>        |[<span data-ttu-id="ce553-134">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="ce553-134">positionDetail</span></span>](positiondetail.md)          | <span data-ttu-id="ce553-135">Содержит подробные сведения о роли пользователя в проекте.</span><span class="sxs-lookup"><span data-stu-id="ce553-135">Contains detail about the user's role on the project.</span></span>                                             |
|<span data-ttu-id="ce553-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ce553-136">displayName</span></span>   |<span data-ttu-id="ce553-137">String</span><span class="sxs-lookup"><span data-stu-id="ce553-137">String</span></span>                                       |<span data-ttu-id="ce553-138">Содержит понятное имя проекта.</span><span class="sxs-lookup"><span data-stu-id="ce553-138">Contains a friendly name for the project.</span></span>                                                         |
|<span data-ttu-id="ce553-139">спонсорами</span><span class="sxs-lookup"><span data-stu-id="ce553-139">sponsors</span></span>      |<span data-ttu-id="ce553-140">Коллекция [релатедперсон](relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="ce553-140">[relatedPerson](relatedperson.md) collection</span></span> | <span data-ttu-id="ce553-141">Пользователь или люди, которые спонсорируют проект.</span><span class="sxs-lookup"><span data-stu-id="ce553-141">The Person or people who sponsored the project.</span></span>                                                         |

## <a name="relationships"></a><span data-ttu-id="ce553-142">Связи</span><span class="sxs-lookup"><span data-stu-id="ce553-142">Relationships</span></span>

<span data-ttu-id="ce553-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ce553-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce553-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ce553-144">JSON representation</span></span>

<span data-ttu-id="ce553-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce553-145">The following is a JSON representation of the resource.</span></span>

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
