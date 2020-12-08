---
title: Тип ресурса Ревиевсеткуери
description: Просмотр запросов Set используется для запроса и отбора данных, хранящихся в представлении "обнаружение электронных данных"
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 7ffea670daffb6c8ce53925096dbd4f2d4986477
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597263"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="64354-103">Тип ресурса Ревиевсеткуери</span><span class="sxs-lookup"><span data-stu-id="64354-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="64354-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64354-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64354-105">Просмотр запросов Set используется для запроса и отбора данных, хранящихся в [представлении](reviewset.md)обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="64354-105">Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="64354-106">Методы</span><span class="sxs-lookup"><span data-stu-id="64354-106">Methods</span></span>

| <span data-ttu-id="64354-107">Метод</span><span class="sxs-lookup"><span data-stu-id="64354-107">Method</span></span>       | <span data-ttu-id="64354-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64354-108">Return Type</span></span> | <span data-ttu-id="64354-109">Описание</span><span class="sxs-lookup"><span data-stu-id="64354-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="64354-110">Перечисление запросов</span><span class="sxs-lookup"><span data-stu-id="64354-110">List queries</span></span>](../api/reviewsetquery-list.md) | <span data-ttu-id="64354-111">Коллекция [ревиевсеткуери](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="64354-111">[reviewSetQuery](reviewsetquery.md) collection</span></span> | <span data-ttu-id="64354-112">Перечисление запросов на набор проверок в наборе рецензирования.</span><span class="sxs-lookup"><span data-stu-id="64354-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="64354-113">Создание запросов</span><span class="sxs-lookup"><span data-stu-id="64354-113">Create queries</span></span>](../api/reviewsetquery-post.md) | [<span data-ttu-id="64354-114">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="64354-114">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="64354-115">Создание запроса на проверку набора.</span><span class="sxs-lookup"><span data-stu-id="64354-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="64354-116">Получение запросов</span><span class="sxs-lookup"><span data-stu-id="64354-116">Get queries</span></span>](../api/reviewsetquery-get.md) | [<span data-ttu-id="64354-117">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="64354-117">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="64354-118">Чтение свойств и связей объекта **ревиевсеткуери** .</span><span class="sxs-lookup"><span data-stu-id="64354-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="64354-119">Запросы на обновление</span><span class="sxs-lookup"><span data-stu-id="64354-119">Update queries</span></span>](../api/reviewsetquery-update.md) | <span data-ttu-id="64354-120">Нет</span><span class="sxs-lookup"><span data-stu-id="64354-120">None</span></span> | <span data-ttu-id="64354-121">Обновление запроса на проверку набора.</span><span class="sxs-lookup"><span data-stu-id="64354-121">Update a review set query.</span></span> |
| [<span data-ttu-id="64354-122">Удаление запросов</span><span class="sxs-lookup"><span data-stu-id="64354-122">Delete queries</span></span>](../api/reviewsetquery-delete.md) | <span data-ttu-id="64354-123">Нет</span><span class="sxs-lookup"><span data-stu-id="64354-123">None</span></span> | <span data-ttu-id="64354-124">Удаление запроса на проверку набора.</span><span class="sxs-lookup"><span data-stu-id="64354-124">Delete review set query.</span></span> |

## <a name="properties"></a><span data-ttu-id="64354-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="64354-125">Properties</span></span>

| <span data-ttu-id="64354-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="64354-126">Property</span></span>     | <span data-ttu-id="64354-127">Тип</span><span class="sxs-lookup"><span data-stu-id="64354-127">Type</span></span>        | <span data-ttu-id="64354-128">Описание</span><span class="sxs-lookup"><span data-stu-id="64354-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="64354-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="64354-129">createdBy</span></span> | [<span data-ttu-id="64354-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="64354-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="64354-131">Пользователь, создавший запрос.</span><span class="sxs-lookup"><span data-stu-id="64354-131">The user who created the query.</span></span> |
| <span data-ttu-id="64354-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64354-132">createdDateTime</span></span> |<span data-ttu-id="64354-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64354-133">DateTimeOffset</span></span>| <span data-ttu-id="64354-134">Время и Дата создания запроса.</span><span class="sxs-lookup"><span data-stu-id="64354-134">The time and date when the query was created.</span></span> <span data-ttu-id="64354-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="64354-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64354-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="64354-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="64354-137">displayName</span><span class="sxs-lookup"><span data-stu-id="64354-137">displayName</span></span> | <span data-ttu-id="64354-138">String</span><span class="sxs-lookup"><span data-stu-id="64354-138">String</span></span> | <span data-ttu-id="64354-139">Имя запроса</span><span class="sxs-lookup"><span data-stu-id="64354-139">The name of the query</span></span>|
| <span data-ttu-id="64354-140">id</span><span class="sxs-lookup"><span data-stu-id="64354-140">id</span></span> |<span data-ttu-id="64354-141">String</span><span class="sxs-lookup"><span data-stu-id="64354-141">String</span></span>| <span data-ttu-id="64354-142">Уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="64354-142">The unique identifier of the query.</span></span> <span data-ttu-id="64354-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64354-143">Read-only.</span></span>|
| <span data-ttu-id="64354-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="64354-144">lastModifiedBy</span></span> | [<span data-ttu-id="64354-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="64354-145">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="64354-146">Пользователь, который последним изменил запрос.</span><span class="sxs-lookup"><span data-stu-id="64354-146">The user who last modified the query.</span></span> |
| <span data-ttu-id="64354-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64354-147">lastModifiedDateTime</span></span> |<span data-ttu-id="64354-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64354-148">DateTimeOffset</span></span> | <span data-ttu-id="64354-149">Дата и время последнего изменения запроса.</span><span class="sxs-lookup"><span data-stu-id="64354-149">The date and time the query was last modified.</span></span> <span data-ttu-id="64354-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="64354-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64354-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="64354-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="64354-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="64354-152">query</span></span> | <span data-ttu-id="64354-153">String</span><span class="sxs-lookup"><span data-stu-id="64354-153">String</span></span> | <span data-ttu-id="64354-154">Строка запроса в запросе KQL (ключевое слово языка запросов).</span><span class="sxs-lookup"><span data-stu-id="64354-154">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="64354-155">Дополнительные сведения см. [в статье Field Metadata Fields in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="64354-155">For details, see [Document metadata fields in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="64354-156">Это поле напрямую сопоставляется с условием ключевых слов.</span><span class="sxs-lookup"><span data-stu-id="64354-156">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="64354-157">Вы можете уточнить поиск с помощью полей, перечисленных в *имени поля с возможностью поиска* , с указанием значений; Например, *Subject: "квартальное финансовое планирование" и дата>= 06/01/2016 и дата<= 07/01/2016*</span><span class="sxs-lookup"><span data-stu-id="64354-157">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span> |

## <a name="relationships"></a><span data-ttu-id="64354-158">Связи</span><span class="sxs-lookup"><span data-stu-id="64354-158">Relationships</span></span>

<span data-ttu-id="64354-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="64354-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64354-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="64354-160">JSON representation</span></span>

<span data-ttu-id="64354-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64354-161">The following is a JSON representation of the resource.</span></span>

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
  "@odata.type": "#microsoft.graph.reviewSetQuery",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
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
