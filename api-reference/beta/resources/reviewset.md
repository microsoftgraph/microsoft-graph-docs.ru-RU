---
title: Тип ресурса reviewSet
description: Представляет статический набор хранимой в электронном виде информации, собираемой для использования в судебных, расследованиях или нормативных запросах.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: b6234fafbf0d6e36d5dcbb4143956447e26d3a0f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153510"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="62d09-103">Тип ресурса reviewSet</span><span class="sxs-lookup"><span data-stu-id="62d09-103">reviewSet resource type</span></span>

<span data-ttu-id="62d09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62d09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62d09-105">Представляет статический набор хранимой в электронном виде информации, собираемой для использования в судебных, расследованиях или нормативных запросах.</span><span class="sxs-lookup"><span data-stu-id="62d09-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="62d09-106">Методы</span><span class="sxs-lookup"><span data-stu-id="62d09-106">Methods</span></span>

| <span data-ttu-id="62d09-107">Метод</span><span class="sxs-lookup"><span data-stu-id="62d09-107">Method</span></span>       | <span data-ttu-id="62d09-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="62d09-108">Return Type</span></span> | <span data-ttu-id="62d09-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62d09-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="62d09-110">Список reviewSet</span><span class="sxs-lookup"><span data-stu-id="62d09-110">List reviewSet</span></span>](../api/reviewset-list.md) | <span data-ttu-id="62d09-111">[Коллекция reviewSet](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="62d09-111">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="62d09-112">Получите коллекцию наборов для проверки.</span><span class="sxs-lookup"><span data-stu-id="62d09-112">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="62d09-113">Get reviewSet</span><span class="sxs-lookup"><span data-stu-id="62d09-113">Get reviewSet</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="62d09-114">reviewSet</span><span class="sxs-lookup"><span data-stu-id="62d09-114">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="62d09-115">Чтение свойств и связей объекта **reviewSet.**</span><span class="sxs-lookup"><span data-stu-id="62d09-115">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="62d09-116">Создание reviewSet</span><span class="sxs-lookup"><span data-stu-id="62d09-116">Create reviewSet</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="62d09-117">reviewSet</span><span class="sxs-lookup"><span data-stu-id="62d09-117">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="62d09-118">Создайте новый набор для проверки.</span><span class="sxs-lookup"><span data-stu-id="62d09-118">Create a new review set.</span></span> |
| [<span data-ttu-id="62d09-119">Список запросов</span><span class="sxs-lookup"><span data-stu-id="62d09-119">List queries</span></span>](../api/reviewsetquery-list.md)|<span data-ttu-id="62d09-120">[Коллекция reviewSetQuery](../resources/reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="62d09-120">[reviewSetQuery](../resources/reviewsetquery.md) collection</span></span>|<span data-ttu-id="62d09-121">Получите ресурсы reviewSetQuery из свойства навигации запросов.</span><span class="sxs-lookup"><span data-stu-id="62d09-121">Get the reviewSetQuery resources from the queries navigation property.</span></span>|
| [<span data-ttu-id="62d09-122">Создание запросов</span><span class="sxs-lookup"><span data-stu-id="62d09-122">Create queries</span></span>](../api/reviewsetquery-post.md)|[<span data-ttu-id="62d09-123">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="62d09-123">reviewSetQuery</span></span>](../resources/reviewsetquery.md)|<span data-ttu-id="62d09-124">Создание объекта reviewSetQuery.</span><span class="sxs-lookup"><span data-stu-id="62d09-124">Create a new reviewSetQuery object.</span></span>|

## <a name="properties"></a><span data-ttu-id="62d09-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="62d09-125">Properties</span></span>

| <span data-ttu-id="62d09-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="62d09-126">Property</span></span>     | <span data-ttu-id="62d09-127">Тип</span><span class="sxs-lookup"><span data-stu-id="62d09-127">Type</span></span>        | <span data-ttu-id="62d09-128">Описание</span><span class="sxs-lookup"><span data-stu-id="62d09-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62d09-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="62d09-129">createdBy</span></span>        | [<span data-ttu-id="62d09-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="62d09-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="62d09-131">Пользователь, создавший набор для проверки.</span><span class="sxs-lookup"><span data-stu-id="62d09-131">The user who created the review set.</span></span> <span data-ttu-id="62d09-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62d09-132">Read-only.</span></span> |
|<span data-ttu-id="62d09-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62d09-133">createdDateTime</span></span>  |<span data-ttu-id="62d09-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d09-134">DateTimeOffset</span></span>| <span data-ttu-id="62d09-135">Дата и время создания набора для проверки.</span><span class="sxs-lookup"><span data-stu-id="62d09-135">The datetime when the review set was created.</span></span> <span data-ttu-id="62d09-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="62d09-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="62d09-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="62d09-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="62d09-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62d09-138">Read-only.</span></span> |
|<span data-ttu-id="62d09-139">displayName</span><span class="sxs-lookup"><span data-stu-id="62d09-139">displayName</span></span>      |<span data-ttu-id="62d09-140">String</span><span class="sxs-lookup"><span data-stu-id="62d09-140">String</span></span>| <span data-ttu-id="62d09-141">Имя набора для проверки.</span><span class="sxs-lookup"><span data-stu-id="62d09-141">The review set name.</span></span> <span data-ttu-id="62d09-142">Имя уникально с максимальным ограничением в 64 символа.</span><span class="sxs-lookup"><span data-stu-id="62d09-142">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="62d09-143">id</span><span class="sxs-lookup"><span data-stu-id="62d09-143">id</span></span>               |<span data-ttu-id="62d09-144">String</span><span class="sxs-lookup"><span data-stu-id="62d09-144">String</span></span>| <span data-ttu-id="62d09-145">Уникальный идентификатор набора для проверки.</span><span class="sxs-lookup"><span data-stu-id="62d09-145">The review set unique identifier.</span></span> <span data-ttu-id="62d09-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="62d09-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="62d09-147">Связи</span><span class="sxs-lookup"><span data-stu-id="62d09-147">Relationships</span></span>

| <span data-ttu-id="62d09-148">Связь</span><span class="sxs-lookup"><span data-stu-id="62d09-148">Relationship</span></span> | <span data-ttu-id="62d09-149">Тип</span><span class="sxs-lookup"><span data-stu-id="62d09-149">Type</span></span>        | <span data-ttu-id="62d09-150">Описание</span><span class="sxs-lookup"><span data-stu-id="62d09-150">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="62d09-151">Проверка запроса набора</span><span class="sxs-lookup"><span data-stu-id="62d09-151">Review set query</span></span> |<span data-ttu-id="62d09-152">[Коллекция reviewSetQuery](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="62d09-152">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="62d09-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="62d09-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62d09-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62d09-155">JSON representation</span></span>

<span data-ttu-id="62d09-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62d09-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSet",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
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
