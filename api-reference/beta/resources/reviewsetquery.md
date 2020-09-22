---
title: Тип ресурса Ревиевсеткуери
description: Просмотр запросов Set используется для запроса и отбора данных, хранящихся в представлении "обнаружение электронных данных"
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: d03fae8340f9513e8fb6a26f409682e72b86842e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026224"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="823aa-103">Тип ресурса Ревиевсеткуери</span><span class="sxs-lookup"><span data-stu-id="823aa-103">reviewSetQuery resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="823aa-104">Просмотр запросов Set используется для запроса и отбора данных, хранящихся в [представлении](reviewset.md)обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="823aa-104">Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="823aa-105">Методы</span><span class="sxs-lookup"><span data-stu-id="823aa-105">Methods</span></span>

| <span data-ttu-id="823aa-106">Метод</span><span class="sxs-lookup"><span data-stu-id="823aa-106">Method</span></span>       | <span data-ttu-id="823aa-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="823aa-107">Return Type</span></span> | <span data-ttu-id="823aa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="823aa-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="823aa-109">Список</span><span class="sxs-lookup"><span data-stu-id="823aa-109">List</span></span>](../api/reviewsetquery-list.md) | <span data-ttu-id="823aa-110">Коллекция [ревиевсеткуери](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="823aa-110">[reviewSetQuery](reviewsetquery.md) collection</span></span> | <span data-ttu-id="823aa-111">Перечисление запросов на набор проверок в наборе рецензирования.</span><span class="sxs-lookup"><span data-stu-id="823aa-111">List the review set queries in a review set.</span></span> |
| <span data-ttu-id="823aa-112">[создание](../api/reviewsetquery-post.md);</span><span class="sxs-lookup"><span data-stu-id="823aa-112">[Create](../api/reviewsetquery-post.md)</span></span> | [<span data-ttu-id="823aa-113">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="823aa-113">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="823aa-114">Создание запроса на проверку набора.</span><span class="sxs-lookup"><span data-stu-id="823aa-114">Create a new review set query.</span></span> |
| <span data-ttu-id="823aa-115">[получение](../api/reviewsetquery-get.md);</span><span class="sxs-lookup"><span data-stu-id="823aa-115">[Get](../api/reviewsetquery-get.md)</span></span> | [<span data-ttu-id="823aa-116">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="823aa-116">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="823aa-117">Чтение свойств и связей объекта **ревиевсеткуери** .</span><span class="sxs-lookup"><span data-stu-id="823aa-117">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="823aa-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="823aa-118">Update</span></span>](../api/reviewsetquery-update.md) | <span data-ttu-id="823aa-119">Нет</span><span class="sxs-lookup"><span data-stu-id="823aa-119">None</span></span> | <span data-ttu-id="823aa-120">Обновление запроса на проверку набора.</span><span class="sxs-lookup"><span data-stu-id="823aa-120">Update a review set query.</span></span> |
| [<span data-ttu-id="823aa-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="823aa-121">Delete</span></span>](../api/reviewsetquery-delete.md) | <span data-ttu-id="823aa-122">Нет</span><span class="sxs-lookup"><span data-stu-id="823aa-122">None</span></span> | <span data-ttu-id="823aa-123">Удаление запроса на проверку набора.</span><span class="sxs-lookup"><span data-stu-id="823aa-123">Delete review set query.</span></span> |

## <a name="properties"></a><span data-ttu-id="823aa-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="823aa-124">Properties</span></span>

| <span data-ttu-id="823aa-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="823aa-125">Property</span></span>     | <span data-ttu-id="823aa-126">Тип</span><span class="sxs-lookup"><span data-stu-id="823aa-126">Type</span></span>        | <span data-ttu-id="823aa-127">Описание</span><span class="sxs-lookup"><span data-stu-id="823aa-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="823aa-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="823aa-128">createdBy</span></span> | [<span data-ttu-id="823aa-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="823aa-129">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="823aa-130">Пользователь, создавший запрос.</span><span class="sxs-lookup"><span data-stu-id="823aa-130">The user who created the query.</span></span> |
| <span data-ttu-id="823aa-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="823aa-131">createdDateTime</span></span> |<span data-ttu-id="823aa-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="823aa-132">DateTimeOffset</span></span>| <span data-ttu-id="823aa-133">Время и Дата создания запроса.</span><span class="sxs-lookup"><span data-stu-id="823aa-133">The time and date when the query was created.</span></span> <span data-ttu-id="823aa-134">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="823aa-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="823aa-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="823aa-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="823aa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="823aa-136">displayName</span></span> | <span data-ttu-id="823aa-137">String</span><span class="sxs-lookup"><span data-stu-id="823aa-137">String</span></span> | <span data-ttu-id="823aa-138">Имя запроса</span><span class="sxs-lookup"><span data-stu-id="823aa-138">The name of the query</span></span>|
| <span data-ttu-id="823aa-139">id</span><span class="sxs-lookup"><span data-stu-id="823aa-139">id</span></span> |<span data-ttu-id="823aa-140">String</span><span class="sxs-lookup"><span data-stu-id="823aa-140">String</span></span>| <span data-ttu-id="823aa-141">Уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="823aa-141">The unique identifier of the query.</span></span> <span data-ttu-id="823aa-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="823aa-142">Read-only.</span></span>|
| <span data-ttu-id="823aa-143">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="823aa-143">lastModifiedBy</span></span> | [<span data-ttu-id="823aa-144">identitySet</span><span class="sxs-lookup"><span data-stu-id="823aa-144">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset) | <span data-ttu-id="823aa-145">Пользователь, который последним изменил запрос.</span><span class="sxs-lookup"><span data-stu-id="823aa-145">The user who last modified the query.</span></span> |
| <span data-ttu-id="823aa-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="823aa-146">lastModifiedDateTime</span></span> |<span data-ttu-id="823aa-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="823aa-147">DateTimeOffset</span></span> | <span data-ttu-id="823aa-148">Дата и время последнего изменения запроса.</span><span class="sxs-lookup"><span data-stu-id="823aa-148">The date and time the query was last modified.</span></span> <span data-ttu-id="823aa-149">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="823aa-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="823aa-150">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="823aa-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="823aa-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="823aa-151">query</span></span> | <span data-ttu-id="823aa-152">String</span><span class="sxs-lookup"><span data-stu-id="823aa-152">String</span></span> | <span data-ttu-id="823aa-153">Строка запроса в запросе KQL (ключевое слово языка запросов).</span><span class="sxs-lookup"><span data-stu-id="823aa-153">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="823aa-154">https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscoveryДополнительные сведения см.</span><span class="sxs-lookup"><span data-stu-id="823aa-154">Please refer to https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery for more details.</span></span>  <span data-ttu-id="823aa-155">Это поле напрямую сопоставляется с условием ключевых слов.</span><span class="sxs-lookup"><span data-stu-id="823aa-155">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="823aa-156">Вы можете уточнить поиск с помощью полей, перечисленных в *имени поля с возможностью поиска* , с указанием значений, например *Subject: "ежеквартальные финансовые операции" и "дата>= 06/01/2016 и дата<= 07/01/2016*</span><span class="sxs-lookup"><span data-stu-id="823aa-156">You can refine searches by using fields listed in the *searchable field name* paired with values, e.g. *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span> |

## <a name="relationships"></a><span data-ttu-id="823aa-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="823aa-157">Relationships</span></span>

<span data-ttu-id="823aa-158">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="823aa-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="823aa-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="823aa-159">JSON representation</span></span>

<span data-ttu-id="823aa-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="823aa-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


