---
title: Тип ресурса Едисковерикасе
description: случаи обнаружения электронных данных — это контейнеры, содержащие custodians, удержания, коллекции, обзоры и экспорты.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 359a74cbf48e0db2b4c3e480b73dfed928232288
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089723"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="3da7c-103">Тип ресурса Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="3da7c-103">ediscoveryCase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3da7c-104">случаи обнаружения электронных данных — это контейнеры, содержащие custodians, удержания, коллекции, обзоры и экспорты.</span><span class="sxs-lookup"><span data-stu-id="3da7c-104">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="3da7c-105">Узнайте больше о обращениях и [Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).</span><span class="sxs-lookup"><span data-stu-id="3da7c-105">Learn more about cases and [Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="3da7c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3da7c-106">Methods</span></span>

| <span data-ttu-id="3da7c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3da7c-107">Method</span></span>       | <span data-ttu-id="3da7c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3da7c-108">Return Type</span></span> | <span data-ttu-id="3da7c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3da7c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3da7c-110">Перечисление</span><span class="sxs-lookup"><span data-stu-id="3da7c-110">List</span></span>](../api/ediscoverycase-list.md) | <span data-ttu-id="3da7c-111">Коллекция [едисковерикасе](ediscoverycase.md)</span><span class="sxs-lookup"><span data-stu-id="3da7c-111">[ediscoveryCase](ediscoverycase.md) collection</span></span> | <span data-ttu-id="3da7c-112">Получение списка дел eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="3da7c-112">Get a list of eDiscovery cases.</span></span>|
| [<span data-ttu-id="3da7c-113">Получение</span><span class="sxs-lookup"><span data-stu-id="3da7c-113">Get</span></span>](../api/ediscoverycase-get.md) | [<span data-ttu-id="3da7c-114">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="3da7c-114">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="3da7c-115">Считывание свойств дел eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="3da7c-115">Read eDiscovery case properties.</span></span> |
| [<span data-ttu-id="3da7c-116">Создание</span><span class="sxs-lookup"><span data-stu-id="3da7c-116">Create</span></span>](../api/ediscoverycase-post.md) | [<span data-ttu-id="3da7c-117">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="3da7c-117">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="3da7c-118">Создание нового **едисковерикасе** путем публикации в коллекции вариантов.</span><span class="sxs-lookup"><span data-stu-id="3da7c-118">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| [<span data-ttu-id="3da7c-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="3da7c-119">Update</span></span>](../api/ediscoverycase-update.md) | [<span data-ttu-id="3da7c-120">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="3da7c-120">ediscoveryCase</span></span>](ediscoverycase.md) | <span data-ttu-id="3da7c-121">Обновление случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="3da7c-121">Update an eDiscovery case.</span></span> |
| <span data-ttu-id="3da7c-122">[удаление](../api/ediscoverycase-delete.md);</span><span class="sxs-lookup"><span data-stu-id="3da7c-122">[Delete](../api/ediscoverycase-delete.md)</span></span> | <span data-ttu-id="3da7c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="3da7c-123">None</span></span> | <span data-ttu-id="3da7c-124">Удаление случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="3da7c-124">Delete an eDiscovery case.</span></span> |

## <a name="properties"></a><span data-ttu-id="3da7c-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="3da7c-125">Properties</span></span>

| <span data-ttu-id="3da7c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3da7c-126">Property</span></span>     | <span data-ttu-id="3da7c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3da7c-127">Type</span></span>        | <span data-ttu-id="3da7c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3da7c-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3da7c-129">клоседби</span><span class="sxs-lookup"><span data-stu-id="3da7c-129">closedBy</span></span>|[<span data-ttu-id="3da7c-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="3da7c-130">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="3da7c-131">Пользователь, который закрыл обращение.</span><span class="sxs-lookup"><span data-stu-id="3da7c-131">The user who closed the case.</span></span>|
|<span data-ttu-id="3da7c-132">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="3da7c-132">closedDateTime</span></span>|<span data-ttu-id="3da7c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3da7c-133">DateTimeOffset</span></span>|<span data-ttu-id="3da7c-134">Дата и время закрытия обращения.</span><span class="sxs-lookup"><span data-stu-id="3da7c-134">The date and time when the case was closed.</span></span> <span data-ttu-id="3da7c-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3da7c-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3da7c-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3da7c-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3da7c-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="3da7c-137">createdBy</span></span>|[<span data-ttu-id="3da7c-138">identitySet</span><span class="sxs-lookup"><span data-stu-id="3da7c-138">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="3da7c-139">Пользователь, создавший обращение.</span><span class="sxs-lookup"><span data-stu-id="3da7c-139">The user who created the case.</span></span>|
|<span data-ttu-id="3da7c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3da7c-140">createdDateTime</span></span>|<span data-ttu-id="3da7c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3da7c-141">DateTimeOffset</span></span>|<span data-ttu-id="3da7c-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3da7c-142">The date and time when the entity was created.</span></span> <span data-ttu-id="3da7c-143">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3da7c-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3da7c-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3da7c-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3da7c-145">description</span><span class="sxs-lookup"><span data-stu-id="3da7c-145">description</span></span>|<span data-ttu-id="3da7c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="3da7c-146">String</span></span>|<span data-ttu-id="3da7c-147">Описание варианта.</span><span class="sxs-lookup"><span data-stu-id="3da7c-147">The case description.</span></span>|
|<span data-ttu-id="3da7c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3da7c-148">displayName</span></span>|<span data-ttu-id="3da7c-149">Строка</span><span class="sxs-lookup"><span data-stu-id="3da7c-149">String</span></span>|<span data-ttu-id="3da7c-150">Имя дела.</span><span class="sxs-lookup"><span data-stu-id="3da7c-150">The case name.</span></span>|
|<span data-ttu-id="3da7c-151">externalId</span><span class="sxs-lookup"><span data-stu-id="3da7c-151">externalId</span></span>|<span data-ttu-id="3da7c-152">String</span><span class="sxs-lookup"><span data-stu-id="3da7c-152">String</span></span>|<span data-ttu-id="3da7c-153">Номер внешнего обращения для ссылки на клиента.</span><span class="sxs-lookup"><span data-stu-id="3da7c-153">The external case number for customer reference.</span></span>|
|<span data-ttu-id="3da7c-154">id</span><span class="sxs-lookup"><span data-stu-id="3da7c-154">id</span></span>|<span data-ttu-id="3da7c-155">Строка</span><span class="sxs-lookup"><span data-stu-id="3da7c-155">String</span></span>| <span data-ttu-id="3da7c-156">Идентификатор для случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="3da7c-156">The ID for the eDiscovery case.</span></span> <span data-ttu-id="3da7c-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3da7c-157">Read-only.</span></span> |
|<span data-ttu-id="3da7c-158">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3da7c-158">lastModifiedBy</span></span>|[<span data-ttu-id="3da7c-159">identitySet</span><span class="sxs-lookup"><span data-stu-id="3da7c-159">identitySet</span></span>](https://docs.microsoft.com/graph/api/resources/identityset)|<span data-ttu-id="3da7c-160">Последний пользователь, изменившего объект.</span><span class="sxs-lookup"><span data-stu-id="3da7c-160">The last user who modified the entity.</span></span>|
|<span data-ttu-id="3da7c-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3da7c-161">lastModifiedDateTime</span></span>|<span data-ttu-id="3da7c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3da7c-162">DateTimeOffset</span></span>| <span data-ttu-id="3da7c-163">Дата и время последнего изменения обращения.</span><span class="sxs-lookup"><span data-stu-id="3da7c-163">The latest date and time when the case was modified.</span></span> <span data-ttu-id="3da7c-164">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3da7c-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3da7c-165">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3da7c-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3da7c-166">status</span><span class="sxs-lookup"><span data-stu-id="3da7c-166">status</span></span>|<span data-ttu-id="3da7c-167">String</span><span class="sxs-lookup"><span data-stu-id="3da7c-167">String</span></span>| <span data-ttu-id="3da7c-168">Состояние обращения.</span><span class="sxs-lookup"><span data-stu-id="3da7c-168">The case status.</span></span> <span data-ttu-id="3da7c-169">Возможные значения: `unknown` , `active` , `pendingDelete` , `closing` , `closed` и `closedWithError` .</span><span class="sxs-lookup"><span data-stu-id="3da7c-169">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="3da7c-170">Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="3da7c-170">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="3da7c-171">значения Касестатус</span><span class="sxs-lookup"><span data-stu-id="3da7c-171">caseStatus values</span></span>

|<span data-ttu-id="3da7c-172">Member</span><span class="sxs-lookup"><span data-stu-id="3da7c-172">Member</span></span>|<span data-ttu-id="3da7c-173">Описание</span><span class="sxs-lookup"><span data-stu-id="3da7c-173">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="3da7c-174">unknown</span><span class="sxs-lookup"><span data-stu-id="3da7c-174">unknown</span></span> | <span data-ttu-id="3da7c-175">Состояние обращения неизвестно.</span><span class="sxs-lookup"><span data-stu-id="3da7c-175">Case status is unknown.</span></span> |
| <span data-ttu-id="3da7c-176">ASP</span><span class="sxs-lookup"><span data-stu-id="3da7c-176">active</span></span> | <span data-ttu-id="3da7c-177">Регистр активен.</span><span class="sxs-lookup"><span data-stu-id="3da7c-177">Case is active.</span></span> |
| <span data-ttu-id="3da7c-178">пендингделете</span><span class="sxs-lookup"><span data-stu-id="3da7c-178">pendingDelete</span></span> | <span data-ttu-id="3da7c-179">Обращение было удалено, но удаление не было полностью транзакционным.</span><span class="sxs-lookup"><span data-stu-id="3da7c-179">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="3da7c-180">крываем</span><span class="sxs-lookup"><span data-stu-id="3da7c-180">closing</span></span> | <span data-ttu-id="3da7c-181">Обращение было закрыто, но операция не была полностью транзакционной.</span><span class="sxs-lookup"><span data-stu-id="3da7c-181">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="3da7c-182">замкнут</span><span class="sxs-lookup"><span data-stu-id="3da7c-182">closed</span></span> | <span data-ttu-id="3da7c-183">Обращение закрывается.</span><span class="sxs-lookup"><span data-stu-id="3da7c-183">The case is closed.</span></span> |
| <span data-ttu-id="3da7c-184">клоседвисеррор</span><span class="sxs-lookup"><span data-stu-id="3da7c-184">closedWithError</span></span> | <span data-ttu-id="3da7c-185">Обращение закрыто, но в этом случае возникли ошибки.</span><span class="sxs-lookup"><span data-stu-id="3da7c-185">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3da7c-186">Связи</span><span class="sxs-lookup"><span data-stu-id="3da7c-186">Relationships</span></span>

| <span data-ttu-id="3da7c-187">Связь</span><span class="sxs-lookup"><span data-stu-id="3da7c-187">Relationship</span></span> | <span data-ttu-id="3da7c-188">Тип</span><span class="sxs-lookup"><span data-stu-id="3da7c-188">Type</span></span>        | <span data-ttu-id="3da7c-189">Описание</span><span class="sxs-lookup"><span data-stu-id="3da7c-189">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3da7c-190">Обзор наборов</span><span class="sxs-lookup"><span data-stu-id="3da7c-190">Review sets</span></span>|<span data-ttu-id="3da7c-191">Коллекция [reviewing](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="3da7c-191">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="3da7c-192">Коллекция наборов проверки в случае.</span><span class="sxs-lookup"><span data-stu-id="3da7c-192">Collection of review sets in the case.</span></span> <span data-ttu-id="3da7c-193">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3da7c-193">Read-only.</span></span> <span data-ttu-id="3da7c-194">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3da7c-194">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3da7c-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3da7c-195">JSON representation</span></span>

<span data-ttu-id="3da7c-196">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3da7c-196">The following is a JSON representation of the resource.</span></span>

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


