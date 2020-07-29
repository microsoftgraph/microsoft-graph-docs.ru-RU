---
title: Тип ресурса Едисковерикасе
description: случаи обнаружения электронных данных — это контейнеры, содержащие custodians, удержания, коллекции, обзоры и экспорты.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 930d04449f24d05d8c9225869506bfc1ed2720aa
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510324"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="88dc7-103">Тип ресурса Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="88dc7-103">ediscoveryCase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88dc7-104">случаи обнаружения электронных данных — это контейнеры, содержащие custodians, удержания, коллекции, обзоры и экспорты.</span><span class="sxs-lookup"><span data-stu-id="88dc7-104">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="88dc7-105">Узнайте больше о обращениях и [Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).</span><span class="sxs-lookup"><span data-stu-id="88dc7-105">Learn more about cases and [Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="88dc7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="88dc7-106">Methods</span></span>

| <span data-ttu-id="88dc7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="88dc7-107">Method</span></span>       | <span data-ttu-id="88dc7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="88dc7-108">Return Type</span></span> | <span data-ttu-id="88dc7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="88dc7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="88dc7-110">Список</span><span class="sxs-lookup"><span data-stu-id="88dc7-110">List</span></span>](../api/ediscoverycase-list.md) | <span data-ttu-id="88dc7-111">Коллекция [едисковерикасе](ediscoverycase.md)</span><span class="sxs-lookup"><span data-stu-id="88dc7-111">[ediscoveryCase](ediscoverycase.md) collection</span></span> | <span data-ttu-id="88dc7-112">Получение списка дел eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="88dc7-112">Get a list of eDiscovery cases.</span></span>|
| <span data-ttu-id="88dc7-113">[получение](../api/ediscoverycase-get.md);</span><span class="sxs-lookup"><span data-stu-id="88dc7-113">[Get](../api/ediscoverycase-get.md)</span></span> | [<span data-ttu-id="88dc7-114">едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="88dc7-114">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="88dc7-115">Считывание свойств дел eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="88dc7-115">Read eDiscovery case properties.</span></span> |
| <span data-ttu-id="88dc7-116">[создание](../api/ediscoverycase-post.md);</span><span class="sxs-lookup"><span data-stu-id="88dc7-116">[Create](../api/ediscoverycase-post.md)</span></span> | [<span data-ttu-id="88dc7-117">едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="88dc7-117">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="88dc7-118">Создание нового **едисковерикасе** путем публикации в коллекции вариантов.</span><span class="sxs-lookup"><span data-stu-id="88dc7-118">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| <span data-ttu-id="88dc7-119">[обновление](../api/ediscoverycase-update.md).</span><span class="sxs-lookup"><span data-stu-id="88dc7-119">[Update](../api/ediscoverycase-update.md)</span></span> | [<span data-ttu-id="88dc7-120">едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="88dc7-120">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="88dc7-121">Обновление случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="88dc7-121">Update an eDiscovery case.</span></span> |
| <span data-ttu-id="88dc7-122">[удаление](../api/ediscoverycase-delete.md);</span><span class="sxs-lookup"><span data-stu-id="88dc7-122">[Delete](../api/ediscoverycase-delete.md)</span></span> | <span data-ttu-id="88dc7-123">Нет</span><span class="sxs-lookup"><span data-stu-id="88dc7-123">None</span></span> | <span data-ttu-id="88dc7-124">Удаление случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="88dc7-124">Delete an eDiscovery case.</span></span> |

## <a name="properties"></a><span data-ttu-id="88dc7-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="88dc7-125">Properties</span></span>

| <span data-ttu-id="88dc7-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="88dc7-126">Property</span></span>     | <span data-ttu-id="88dc7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="88dc7-127">Type</span></span>        | <span data-ttu-id="88dc7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="88dc7-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="88dc7-129">клоседби</span><span class="sxs-lookup"><span data-stu-id="88dc7-129">closedBy</span></span>|[<span data-ttu-id="88dc7-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="88dc7-130">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="88dc7-131">Пользователь, который закрыл обращение.</span><span class="sxs-lookup"><span data-stu-id="88dc7-131">The user who closed the case.</span></span>|
|<span data-ttu-id="88dc7-132">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="88dc7-132">closedDateTime</span></span>|<span data-ttu-id="88dc7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88dc7-133">DateTimeOffset</span></span>|<span data-ttu-id="88dc7-134">Дата и время закрытия обращения.</span><span class="sxs-lookup"><span data-stu-id="88dc7-134">The date and time when the case was closed.</span></span> <span data-ttu-id="88dc7-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="88dc7-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88dc7-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="88dc7-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="88dc7-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="88dc7-137">createdBy</span></span>|[<span data-ttu-id="88dc7-138">identitySet</span><span class="sxs-lookup"><span data-stu-id="88dc7-138">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="88dc7-139">Пользователь, создавший обращение.</span><span class="sxs-lookup"><span data-stu-id="88dc7-139">The user who created the case.</span></span>|
|<span data-ttu-id="88dc7-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88dc7-140">createdDateTime</span></span>|<span data-ttu-id="88dc7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88dc7-141">DateTimeOffset</span></span>|<span data-ttu-id="88dc7-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="88dc7-142">The date and time when the entity was created.</span></span> <span data-ttu-id="88dc7-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="88dc7-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88dc7-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="88dc7-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="88dc7-145">description</span><span class="sxs-lookup"><span data-stu-id="88dc7-145">description</span></span>|<span data-ttu-id="88dc7-146">Строка</span><span class="sxs-lookup"><span data-stu-id="88dc7-146">String</span></span>|<span data-ttu-id="88dc7-147">Описание варианта.</span><span class="sxs-lookup"><span data-stu-id="88dc7-147">The case description.</span></span>|
|<span data-ttu-id="88dc7-148">displayName</span><span class="sxs-lookup"><span data-stu-id="88dc7-148">displayName</span></span>|<span data-ttu-id="88dc7-149">Строка</span><span class="sxs-lookup"><span data-stu-id="88dc7-149">String</span></span>|<span data-ttu-id="88dc7-150">Имя дела.</span><span class="sxs-lookup"><span data-stu-id="88dc7-150">The case name.</span></span>|
|<span data-ttu-id="88dc7-151">externalId</span><span class="sxs-lookup"><span data-stu-id="88dc7-151">externalId</span></span>|<span data-ttu-id="88dc7-152">String</span><span class="sxs-lookup"><span data-stu-id="88dc7-152">String</span></span>|<span data-ttu-id="88dc7-153">Номер внешнего обращения для ссылки на клиента.</span><span class="sxs-lookup"><span data-stu-id="88dc7-153">The external case number for customer reference.</span></span>|
|<span data-ttu-id="88dc7-154">id</span><span class="sxs-lookup"><span data-stu-id="88dc7-154">id</span></span>|<span data-ttu-id="88dc7-155">Строка</span><span class="sxs-lookup"><span data-stu-id="88dc7-155">String</span></span>| <span data-ttu-id="88dc7-156">Идентификатор для случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="88dc7-156">The ID for the eDiscovery case.</span></span> <span data-ttu-id="88dc7-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88dc7-157">Read-only.</span></span> |
|<span data-ttu-id="88dc7-158">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="88dc7-158">lastModifiedBy</span></span>|[<span data-ttu-id="88dc7-159">identitySet</span><span class="sxs-lookup"><span data-stu-id="88dc7-159">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="88dc7-160">Последний пользователь, изменившего объект.</span><span class="sxs-lookup"><span data-stu-id="88dc7-160">The last user who modified the entity.</span></span>|
|<span data-ttu-id="88dc7-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88dc7-161">lastModifiedDateTime</span></span>|<span data-ttu-id="88dc7-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88dc7-162">DateTimeOffset</span></span>| <span data-ttu-id="88dc7-163">Дата и время последнего изменения обращения.</span><span class="sxs-lookup"><span data-stu-id="88dc7-163">The latest date and time when the case was modified.</span></span> <span data-ttu-id="88dc7-164">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="88dc7-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88dc7-165">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="88dc7-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="88dc7-166">status</span><span class="sxs-lookup"><span data-stu-id="88dc7-166">status</span></span>|<span data-ttu-id="88dc7-167">String</span><span class="sxs-lookup"><span data-stu-id="88dc7-167">String</span></span>| <span data-ttu-id="88dc7-168">Состояние обращения.</span><span class="sxs-lookup"><span data-stu-id="88dc7-168">The case status.</span></span> <span data-ttu-id="88dc7-169">Возможные значения: `unknown` , `active` , `pendingDelete` , `closing` , `closed` и `closedWithError` .</span><span class="sxs-lookup"><span data-stu-id="88dc7-169">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="88dc7-170">Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="88dc7-170">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="88dc7-171">значения Касестатус</span><span class="sxs-lookup"><span data-stu-id="88dc7-171">caseStatus values</span></span>

|<span data-ttu-id="88dc7-172">Member</span><span class="sxs-lookup"><span data-stu-id="88dc7-172">Member</span></span>|<span data-ttu-id="88dc7-173">Описание</span><span class="sxs-lookup"><span data-stu-id="88dc7-173">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="88dc7-174">unknown</span><span class="sxs-lookup"><span data-stu-id="88dc7-174">unknown</span></span> | <span data-ttu-id="88dc7-175">Состояние обращения неизвестно.</span><span class="sxs-lookup"><span data-stu-id="88dc7-175">Case status is unknown.</span></span> |
| <span data-ttu-id="88dc7-176">ASP</span><span class="sxs-lookup"><span data-stu-id="88dc7-176">active</span></span> | <span data-ttu-id="88dc7-177">Регистр активен.</span><span class="sxs-lookup"><span data-stu-id="88dc7-177">Case is active.</span></span> |
| <span data-ttu-id="88dc7-178">пендингделете</span><span class="sxs-lookup"><span data-stu-id="88dc7-178">pendingDelete</span></span> | <span data-ttu-id="88dc7-179">Обращение было удалено, но удаление не было полностью транзакционным.</span><span class="sxs-lookup"><span data-stu-id="88dc7-179">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="88dc7-180">крываем</span><span class="sxs-lookup"><span data-stu-id="88dc7-180">closing</span></span> | <span data-ttu-id="88dc7-181">Обращение было закрыто, но операция не была полностью транзакционной.</span><span class="sxs-lookup"><span data-stu-id="88dc7-181">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="88dc7-182">замкнут</span><span class="sxs-lookup"><span data-stu-id="88dc7-182">closed</span></span> | <span data-ttu-id="88dc7-183">Обращение закрывается.</span><span class="sxs-lookup"><span data-stu-id="88dc7-183">The case is closed.</span></span> |
| <span data-ttu-id="88dc7-184">клоседвисеррор</span><span class="sxs-lookup"><span data-stu-id="88dc7-184">closedWithError</span></span> | <span data-ttu-id="88dc7-185">Обращение закрыто, но в этом случае возникли ошибки.</span><span class="sxs-lookup"><span data-stu-id="88dc7-185">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="88dc7-186">Связи</span><span class="sxs-lookup"><span data-stu-id="88dc7-186">Relationships</span></span>

| <span data-ttu-id="88dc7-187">Связь</span><span class="sxs-lookup"><span data-stu-id="88dc7-187">Relationship</span></span> | <span data-ttu-id="88dc7-188">Тип</span><span class="sxs-lookup"><span data-stu-id="88dc7-188">Type</span></span>        | <span data-ttu-id="88dc7-189">Описание</span><span class="sxs-lookup"><span data-stu-id="88dc7-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="88dc7-190">Обзор наборов</span><span class="sxs-lookup"><span data-stu-id="88dc7-190">Review sets</span></span>|<span data-ttu-id="88dc7-191">Коллекция [reviewing](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="88dc7-191">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="88dc7-192">Коллекция наборов проверки в случае.</span><span class="sxs-lookup"><span data-stu-id="88dc7-192">Collection of review sets in the case.</span></span> <span data-ttu-id="88dc7-193">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88dc7-193">Read-only.</span></span> <span data-ttu-id="88dc7-194">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="88dc7-194">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88dc7-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88dc7-195">JSON representation</span></span>

<span data-ttu-id="88dc7-196">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88dc7-196">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "closedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "closedDateTime": "String (timestamp)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "status": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ediscoveryCase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
