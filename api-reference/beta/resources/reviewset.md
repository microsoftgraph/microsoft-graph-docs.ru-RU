---
title: Тип ресурса Review
description: Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 374984f2d44050c1332ec016f83a1ccdea909ba0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510168"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="258f8-103">Тип ресурса Review</span><span class="sxs-lookup"><span data-stu-id="258f8-103">reviewSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="258f8-104">Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.</span><span class="sxs-lookup"><span data-stu-id="258f8-104">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="258f8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="258f8-105">Methods</span></span>

| <span data-ttu-id="258f8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="258f8-106">Method</span></span>       | <span data-ttu-id="258f8-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="258f8-107">Return Type</span></span> | <span data-ttu-id="258f8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="258f8-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="258f8-109">Список</span><span class="sxs-lookup"><span data-stu-id="258f8-109">List</span></span>](../api/reviewset-list.md) | <span data-ttu-id="258f8-110">Коллекция [reviewing](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="258f8-110">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="258f8-111">Получение коллекции наборов проверки.</span><span class="sxs-lookup"><span data-stu-id="258f8-111">Get a collection of review sets.</span></span> |
| <span data-ttu-id="258f8-112">[получение](../api/reviewset-get.md);</span><span class="sxs-lookup"><span data-stu-id="258f8-112">[Get](../api/reviewset-get.md)</span></span> | [<span data-ttu-id="258f8-113">проверяющий</span><span class="sxs-lookup"><span data-stu-id="258f8-113">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="258f8-114">Считывание свойств и связей объекта **reviewing** .</span><span class="sxs-lookup"><span data-stu-id="258f8-114">Read the properties and relationships of a **reviewSet** object.</span></span> |
| <span data-ttu-id="258f8-115">[создание](../api/reviewset-post.md);</span><span class="sxs-lookup"><span data-stu-id="258f8-115">[Create](../api/reviewset-post.md)</span></span> | [<span data-ttu-id="258f8-116">проверяющий</span><span class="sxs-lookup"><span data-stu-id="258f8-116">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="258f8-117">Создайте новый набор рецензирования.</span><span class="sxs-lookup"><span data-stu-id="258f8-117">Create a new review set.</span></span> |

## <a name="properties"></a><span data-ttu-id="258f8-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="258f8-118">Properties</span></span>

| <span data-ttu-id="258f8-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="258f8-119">Property</span></span>     | <span data-ttu-id="258f8-120">Тип</span><span class="sxs-lookup"><span data-stu-id="258f8-120">Type</span></span>        | <span data-ttu-id="258f8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="258f8-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="258f8-122">createdBy</span><span class="sxs-lookup"><span data-stu-id="258f8-122">createdBy</span></span>| [<span data-ttu-id="258f8-123">identitySet</span><span class="sxs-lookup"><span data-stu-id="258f8-123">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="258f8-124">Пользователь, создавший набор проверки.</span><span class="sxs-lookup"><span data-stu-id="258f8-124">The user who created the review set.</span></span> <span data-ttu-id="258f8-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="258f8-125">Read-only.</span></span> |
|<span data-ttu-id="258f8-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="258f8-126">createdDateTime</span></span>|<span data-ttu-id="258f8-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="258f8-127">DateTimeOffset</span></span>| <span data-ttu-id="258f8-128">Дата и время создания набора проверки.</span><span class="sxs-lookup"><span data-stu-id="258f8-128">The datetime when the review set was created.</span></span> <span data-ttu-id="258f8-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="258f8-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="258f8-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="258f8-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="258f8-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="258f8-131">Read-only.</span></span> |
|<span data-ttu-id="258f8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="258f8-132">displayName</span></span>|<span data-ttu-id="258f8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="258f8-133">String</span></span>| <span data-ttu-id="258f8-134">Имя набора проверки.</span><span class="sxs-lookup"><span data-stu-id="258f8-134">The review set name.</span></span> <span data-ttu-id="258f8-135">Имя уникально с максимальным ограничением в 64 символов.</span><span class="sxs-lookup"><span data-stu-id="258f8-135">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="258f8-136">id</span><span class="sxs-lookup"><span data-stu-id="258f8-136">id</span></span>|<span data-ttu-id="258f8-137">String</span><span class="sxs-lookup"><span data-stu-id="258f8-137">String</span></span>| <span data-ttu-id="258f8-138">Уникальный идентификатор набора проверки.</span><span class="sxs-lookup"><span data-stu-id="258f8-138">The review set unique identifier.</span></span> <span data-ttu-id="258f8-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="258f8-139">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="258f8-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="258f8-140">Relationships</span></span>

| <span data-ttu-id="258f8-141">Связь</span><span class="sxs-lookup"><span data-stu-id="258f8-141">Relationship</span></span> | <span data-ttu-id="258f8-142">Тип</span><span class="sxs-lookup"><span data-stu-id="258f8-142">Type</span></span>        | <span data-ttu-id="258f8-143">Описание</span><span class="sxs-lookup"><span data-stu-id="258f8-143">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="258f8-144">Просмотр запроса Set</span><span class="sxs-lookup"><span data-stu-id="258f8-144">Review set query</span></span> |<span data-ttu-id="258f8-145">Коллекция [ревиевсеткуери](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="258f8-145">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="258f8-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="258f8-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="258f8-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="258f8-148">JSON representation</span></span>

<span data-ttu-id="258f8-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="258f8-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
