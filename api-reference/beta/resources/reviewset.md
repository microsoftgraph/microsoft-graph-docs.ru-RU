---
title: Тип ресурса Review
description: Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f1bf04c8357fbd57876b460848c549b3edd6f1f7
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48400746"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="42140-103">Тип ресурса Review</span><span class="sxs-lookup"><span data-stu-id="42140-103">reviewSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42140-104">Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.</span><span class="sxs-lookup"><span data-stu-id="42140-104">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="42140-105">Методы</span><span class="sxs-lookup"><span data-stu-id="42140-105">Methods</span></span>

| <span data-ttu-id="42140-106">Метод</span><span class="sxs-lookup"><span data-stu-id="42140-106">Method</span></span>       | <span data-ttu-id="42140-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="42140-107">Return Type</span></span> | <span data-ttu-id="42140-108">Описание</span><span class="sxs-lookup"><span data-stu-id="42140-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="42140-109">Список</span><span class="sxs-lookup"><span data-stu-id="42140-109">List</span></span>](../api/reviewset-list.md) | <span data-ttu-id="42140-110">Коллекция [reviewing](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="42140-110">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="42140-111">Получение коллекции наборов проверки.</span><span class="sxs-lookup"><span data-stu-id="42140-111">Get a collection of review sets.</span></span> |
| <span data-ttu-id="42140-112">[получение](../api/reviewset-get.md);</span><span class="sxs-lookup"><span data-stu-id="42140-112">[Get](../api/reviewset-get.md)</span></span> | [<span data-ttu-id="42140-113">reviewSet</span><span class="sxs-lookup"><span data-stu-id="42140-113">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="42140-114">Считывание свойств и связей объекта **reviewing** .</span><span class="sxs-lookup"><span data-stu-id="42140-114">Read the properties and relationships of a **reviewSet** object.</span></span> |
| <span data-ttu-id="42140-115">[создание](../api/reviewset-post.md);</span><span class="sxs-lookup"><span data-stu-id="42140-115">[Create](../api/reviewset-post.md)</span></span> | [<span data-ttu-id="42140-116">reviewSet</span><span class="sxs-lookup"><span data-stu-id="42140-116">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="42140-117">Создайте новый набор рецензирования.</span><span class="sxs-lookup"><span data-stu-id="42140-117">Create a new review set.</span></span> |

## <a name="properties"></a><span data-ttu-id="42140-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="42140-118">Properties</span></span>

| <span data-ttu-id="42140-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="42140-119">Property</span></span>     | <span data-ttu-id="42140-120">Тип</span><span class="sxs-lookup"><span data-stu-id="42140-120">Type</span></span>        | <span data-ttu-id="42140-121">Описание</span><span class="sxs-lookup"><span data-stu-id="42140-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42140-122">createdBy</span><span class="sxs-lookup"><span data-stu-id="42140-122">createdBy</span></span>| [<span data-ttu-id="42140-123">identitySet</span><span class="sxs-lookup"><span data-stu-id="42140-123">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="42140-124">Пользователь, создавший набор проверки.</span><span class="sxs-lookup"><span data-stu-id="42140-124">The user who created the review set.</span></span> <span data-ttu-id="42140-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42140-125">Read-only.</span></span> |
|<span data-ttu-id="42140-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42140-126">createdDateTime</span></span>|<span data-ttu-id="42140-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42140-127">DateTimeOffset</span></span>| <span data-ttu-id="42140-128">Дата и время создания набора проверки.</span><span class="sxs-lookup"><span data-stu-id="42140-128">The datetime when the review set was created.</span></span> <span data-ttu-id="42140-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="42140-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="42140-130">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="42140-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="42140-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42140-131">Read-only.</span></span> |
|<span data-ttu-id="42140-132">displayName</span><span class="sxs-lookup"><span data-stu-id="42140-132">displayName</span></span>|<span data-ttu-id="42140-133">String</span><span class="sxs-lookup"><span data-stu-id="42140-133">String</span></span>| <span data-ttu-id="42140-134">Имя набора проверки.</span><span class="sxs-lookup"><span data-stu-id="42140-134">The review set name.</span></span> <span data-ttu-id="42140-135">Имя уникально с максимальным ограничением в 64 символов.</span><span class="sxs-lookup"><span data-stu-id="42140-135">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="42140-136">id</span><span class="sxs-lookup"><span data-stu-id="42140-136">id</span></span>|<span data-ttu-id="42140-137">String</span><span class="sxs-lookup"><span data-stu-id="42140-137">String</span></span>| <span data-ttu-id="42140-138">Уникальный идентификатор набора проверки.</span><span class="sxs-lookup"><span data-stu-id="42140-138">The review set unique identifier.</span></span> <span data-ttu-id="42140-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42140-139">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="42140-140">Связи</span><span class="sxs-lookup"><span data-stu-id="42140-140">Relationships</span></span>

| <span data-ttu-id="42140-141">Связь</span><span class="sxs-lookup"><span data-stu-id="42140-141">Relationship</span></span> | <span data-ttu-id="42140-142">Тип</span><span class="sxs-lookup"><span data-stu-id="42140-142">Type</span></span>        | <span data-ttu-id="42140-143">Описание</span><span class="sxs-lookup"><span data-stu-id="42140-143">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="42140-144">Просмотр запроса Set</span><span class="sxs-lookup"><span data-stu-id="42140-144">Review set query</span></span> |<span data-ttu-id="42140-145">Коллекция [ревиевсеткуери](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="42140-145">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="42140-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="42140-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42140-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42140-148">JSON representation</span></span>

<span data-ttu-id="42140-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42140-149">The following is a JSON representation of the resource.</span></span>

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