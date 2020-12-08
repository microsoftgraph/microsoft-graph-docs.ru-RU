---
title: Тип ресурса Едисковерикасе
description: случаи обнаружения электронных данных — это контейнеры, содержащие custodians, удержания, коллекции, обзоры и экспорты.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 12d2901ff6a61213affd14d681c0ec7b6a74470c
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597405"
---
# <a name="ediscoverycase-resource-type"></a><span data-ttu-id="6a0e7-103">Тип ресурса Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="6a0e7-103">ediscoveryCase resource type</span></span>

<span data-ttu-id="6a0e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a0e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a0e7-105">случаи обнаружения электронных данных — это контейнеры, содержащие custodians, удержания, коллекции, обзоры и экспорты.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-105">eDiscovery cases are containers that contain custodians, holds, collections, review sets, and exports.</span></span>  <span data-ttu-id="6a0e7-106">Узнайте больше о обращениях и [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20).</span><span class="sxs-lookup"><span data-stu-id="6a0e7-106">Learn more about cases and [Advanced eDiscovery](/microsoft-365/compliance/overview-ediscovery-20).</span></span>

## <a name="methods"></a><span data-ttu-id="6a0e7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6a0e7-107">Methods</span></span>

| <span data-ttu-id="6a0e7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6a0e7-108">Method</span></span>       | <span data-ttu-id="6a0e7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6a0e7-109">Return Type</span></span> | <span data-ttu-id="6a0e7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a0e7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6a0e7-111">Список Едисковерикасес</span><span class="sxs-lookup"><span data-stu-id="6a0e7-111">List ediscoveryCases</span></span>](../api/ediscoverycase-list.md)          | <span data-ttu-id="6a0e7-112">Коллекция [едисковерикасе](ediscoverycase.md)</span><span class="sxs-lookup"><span data-stu-id="6a0e7-112">[ediscoveryCase](ediscoverycase.md) collection</span></span>   | <span data-ttu-id="6a0e7-113">Получение списка дел eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-113">Get a list of eDiscovery cases.</span></span>|
| [<span data-ttu-id="6a0e7-114">Получение Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="6a0e7-114">Get ediscoveryCase</span></span>](../api/ediscoverycase-get.md)            | [<span data-ttu-id="6a0e7-115">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="6a0e7-115">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="6a0e7-116">Считывание свойств дел eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-116">Read eDiscovery case properties.</span></span> |
| [<span data-ttu-id="6a0e7-117">Создание Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="6a0e7-117">Create ediscoveryCase</span></span>](../api/ediscoverycase-post.md)        | [<span data-ttu-id="6a0e7-118">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="6a0e7-118">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="6a0e7-119">Создание нового **едисковерикасе** путем публикации в коллекции вариантов.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-119">Create a new **ediscoveryCase** by posting to the cases collection.</span></span> |
| [<span data-ttu-id="6a0e7-120">Обновление Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="6a0e7-120">Update ediscoveryCase</span></span>](../api/ediscoverycase-update.md)      | [<span data-ttu-id="6a0e7-121">ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="6a0e7-121">ediscoveryCase</span></span>](ediscoverycase.md)               | <span data-ttu-id="6a0e7-122">Обновление случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-122">Update an eDiscovery case.</span></span> |
| [<span data-ttu-id="6a0e7-123">Удаление Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="6a0e7-123">Delete ediscoveryCase</span></span>](../api/ediscoverycase-delete.md)      | <span data-ttu-id="6a0e7-124">Нет</span><span class="sxs-lookup"><span data-stu-id="6a0e7-124">None</span></span>                                              | <span data-ttu-id="6a0e7-125">Удаление случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-125">Delete an eDiscovery case.</span></span> |
| [<span data-ttu-id="6a0e7-126">Закрыть Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="6a0e7-126">Close ediscoveryCase</span></span>](../api/ediscoverycase-close.md)        | <span data-ttu-id="6a0e7-127">Нет</span><span class="sxs-lookup"><span data-stu-id="6a0e7-127">None</span></span>                                              | <span data-ttu-id="6a0e7-128">Закройте дело обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-128">Close an eDiscovery case.</span></span> |
| [<span data-ttu-id="6a0e7-129">Повторное открытие Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="6a0e7-129">Reopen ediscoveryCase</span></span>](../api/ediscoverycase-reopen.md)      | <span data-ttu-id="6a0e7-130">Нет</span><span class="sxs-lookup"><span data-stu-id="6a0e7-130">None</span></span>                                              | <span data-ttu-id="6a0e7-131">Повторное открытие закрытого случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-131">Reopen a closed eDiscovery case.</span></span>|
| [<span data-ttu-id="6a0e7-132">Список custodians</span><span class="sxs-lookup"><span data-stu-id="6a0e7-132">List custodians</span></span>](../api/custodian-get.md)   | <span data-ttu-id="6a0e7-133">Коллекция [хранитель](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="6a0e7-133">[custodian](../resources/custodian.md) collection</span></span> |<span data-ttu-id="6a0e7-134">Получение ресурсов хранитель из свойства навигации custodians.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-134">Get the custodian resources from the custodians navigation property.</span></span>|
| [<span data-ttu-id="6a0e7-135">Создание custodians</span><span class="sxs-lookup"><span data-stu-id="6a0e7-135">Create custodians</span></span>](../api/ediscoverycase-post-custodians.md)  | [<span data-ttu-id="6a0e7-136">Хранитель</span><span class="sxs-lookup"><span data-stu-id="6a0e7-136">custodian</span></span>](../resources/custodian.md)           |<span data-ttu-id="6a0e7-137">Создание нового объекта хранитель.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-137">Create a new custodian object.</span></span>|
| [<span data-ttu-id="6a0e7-138">Список Ревиевсетс</span><span class="sxs-lookup"><span data-stu-id="6a0e7-138">List reviewSets</span></span>](../api/reviewset-list.md)   | <span data-ttu-id="6a0e7-139">Коллекция [reviewing](../resources/reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="6a0e7-139">[reviewSet](../resources/reviewset.md) collection</span></span> | <span data-ttu-id="6a0e7-140">Получение ресурсов перепредставления из свойства навигации Ревиевсетс.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-140">Get the reviewSet resources from the reviewSets navigation property.</span></span>|
| [<span data-ttu-id="6a0e7-141">Создание Ревиевсетс</span><span class="sxs-lookup"><span data-stu-id="6a0e7-141">Create reviewSets</span></span>](../api/reviewset-post.md)  | [<span data-ttu-id="6a0e7-142">reviewSet</span><span class="sxs-lookup"><span data-stu-id="6a0e7-142">reviewSet</span></span>](../resources/reviewset.md)           | <span data-ttu-id="6a0e7-143">Создайте новый объект Review.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-143">Create a new reviewSet object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a0e7-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a0e7-144">Properties</span></span>

| <span data-ttu-id="6a0e7-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a0e7-145">Property</span></span>     | <span data-ttu-id="6a0e7-146">Тип</span><span class="sxs-lookup"><span data-stu-id="6a0e7-146">Type</span></span>        | <span data-ttu-id="6a0e7-147">Описание</span><span class="sxs-lookup"><span data-stu-id="6a0e7-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a0e7-148">клоседби</span><span class="sxs-lookup"><span data-stu-id="6a0e7-148">closedBy</span></span>|[<span data-ttu-id="6a0e7-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="6a0e7-149">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="6a0e7-150">Пользователь, который закрыл обращение.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-150">The user who closed the case.</span></span>|
|<span data-ttu-id="6a0e7-151">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0e7-151">closedDateTime</span></span>|<span data-ttu-id="6a0e7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a0e7-152">DateTimeOffset</span></span>|<span data-ttu-id="6a0e7-153">Дата и время закрытия обращения.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-153">The date and time when the case was closed.</span></span> <span data-ttu-id="6a0e7-154">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6a0e7-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a0e7-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6a0e7-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="6a0e7-156">createdBy</span></span>|[<span data-ttu-id="6a0e7-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="6a0e7-157">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="6a0e7-158">Пользователь, создавший обращение.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-158">The user who created the case.</span></span>|
|<span data-ttu-id="6a0e7-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0e7-159">createdDateTime</span></span>|<span data-ttu-id="6a0e7-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a0e7-160">DateTimeOffset</span></span>|<span data-ttu-id="6a0e7-161">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-161">The date and time when the entity was created.</span></span> <span data-ttu-id="6a0e7-162">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6a0e7-162">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a0e7-163">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-163">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6a0e7-164">description</span><span class="sxs-lookup"><span data-stu-id="6a0e7-164">description</span></span>|<span data-ttu-id="6a0e7-165">String</span><span class="sxs-lookup"><span data-stu-id="6a0e7-165">String</span></span>|<span data-ttu-id="6a0e7-166">Описание варианта.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-166">The case description.</span></span>|
|<span data-ttu-id="6a0e7-167">displayName</span><span class="sxs-lookup"><span data-stu-id="6a0e7-167">displayName</span></span>|<span data-ttu-id="6a0e7-168">String</span><span class="sxs-lookup"><span data-stu-id="6a0e7-168">String</span></span>|<span data-ttu-id="6a0e7-169">Имя дела.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-169">The case name.</span></span>|
|<span data-ttu-id="6a0e7-170">externalId</span><span class="sxs-lookup"><span data-stu-id="6a0e7-170">externalId</span></span>|<span data-ttu-id="6a0e7-171">String</span><span class="sxs-lookup"><span data-stu-id="6a0e7-171">String</span></span>|<span data-ttu-id="6a0e7-172">Номер внешнего обращения для ссылки на клиента.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-172">The external case number for customer reference.</span></span>|
|<span data-ttu-id="6a0e7-173">id</span><span class="sxs-lookup"><span data-stu-id="6a0e7-173">id</span></span>|<span data-ttu-id="6a0e7-174">String</span><span class="sxs-lookup"><span data-stu-id="6a0e7-174">String</span></span>| <span data-ttu-id="6a0e7-175">Идентификатор для случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-175">The ID for the eDiscovery case.</span></span> <span data-ttu-id="6a0e7-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-176">Read-only.</span></span> |
|<span data-ttu-id="6a0e7-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6a0e7-177">lastModifiedBy</span></span>|[<span data-ttu-id="6a0e7-178">identitySet</span><span class="sxs-lookup"><span data-stu-id="6a0e7-178">identitySet</span></span>](/graph/api/resources/identityset)|<span data-ttu-id="6a0e7-179">Последний пользователь, изменившего объект.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-179">The last user who modified the entity.</span></span>|
|<span data-ttu-id="6a0e7-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0e7-180">lastModifiedDateTime</span></span>|<span data-ttu-id="6a0e7-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a0e7-181">DateTimeOffset</span></span>| <span data-ttu-id="6a0e7-182">Дата и время последнего изменения обращения.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-182">The latest date and time when the case was modified.</span></span> <span data-ttu-id="6a0e7-183">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6a0e7-183">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a0e7-184">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-184">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6a0e7-185">status</span><span class="sxs-lookup"><span data-stu-id="6a0e7-185">status</span></span>|<span data-ttu-id="6a0e7-186">String</span><span class="sxs-lookup"><span data-stu-id="6a0e7-186">String</span></span>| <span data-ttu-id="6a0e7-187">Состояние обращения.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-187">The case status.</span></span> <span data-ttu-id="6a0e7-188">Возможные значения: `unknown` , `active` , `pendingDelete` , `closing` , `closed` и `closedWithError` .</span><span class="sxs-lookup"><span data-stu-id="6a0e7-188">Possible values are `unknown`, `active`, `pendingDelete`, `closing`, `closed`, and `closedWithError`.</span></span> <span data-ttu-id="6a0e7-189">Дополнительные сведения см. в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-189">For details see the following table.</span></span>|

### <a name="casestatus-values"></a><span data-ttu-id="6a0e7-190">значения Касестатус</span><span class="sxs-lookup"><span data-stu-id="6a0e7-190">caseStatus values</span></span>

|<span data-ttu-id="6a0e7-191">Member</span><span class="sxs-lookup"><span data-stu-id="6a0e7-191">Member</span></span>|<span data-ttu-id="6a0e7-192">Описание</span><span class="sxs-lookup"><span data-stu-id="6a0e7-192">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="6a0e7-193">unknown</span><span class="sxs-lookup"><span data-stu-id="6a0e7-193">unknown</span></span> | <span data-ttu-id="6a0e7-194">Состояние обращения неизвестно.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-194">Case status is unknown.</span></span> |
| <span data-ttu-id="6a0e7-195">ASP</span><span class="sxs-lookup"><span data-stu-id="6a0e7-195">active</span></span> | <span data-ttu-id="6a0e7-196">Регистр активен.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-196">Case is active.</span></span> |
| <span data-ttu-id="6a0e7-197">пендингделете</span><span class="sxs-lookup"><span data-stu-id="6a0e7-197">pendingDelete</span></span> | <span data-ttu-id="6a0e7-198">Обращение было удалено, но удаление не было полностью транзакционным.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-198">Case was deleted, but the delete has not been fully transacted.</span></span> |
| <span data-ttu-id="6a0e7-199">крываем</span><span class="sxs-lookup"><span data-stu-id="6a0e7-199">closing</span></span> | <span data-ttu-id="6a0e7-200">Обращение было закрыто, но операция не была полностью транзакционной.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-200">Case was closed, but the operation has not been fully transacted.</span></span> |
| <span data-ttu-id="6a0e7-201">замкнут</span><span class="sxs-lookup"><span data-stu-id="6a0e7-201">closed</span></span> | <span data-ttu-id="6a0e7-202">Обращение закрывается.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-202">The case is closed.</span></span> |
| <span data-ttu-id="6a0e7-203">клоседвисеррор</span><span class="sxs-lookup"><span data-stu-id="6a0e7-203">closedWithError</span></span> | <span data-ttu-id="6a0e7-204">Обращение закрыто, но в этом случае возникли ошибки.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-204">The case is closed, but there were errors releasing holds in the case.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6a0e7-205">Связи</span><span class="sxs-lookup"><span data-stu-id="6a0e7-205">Relationships</span></span>

| <span data-ttu-id="6a0e7-206">Связь</span><span class="sxs-lookup"><span data-stu-id="6a0e7-206">Relationship</span></span> | <span data-ttu-id="6a0e7-207">Тип</span><span class="sxs-lookup"><span data-stu-id="6a0e7-207">Type</span></span>        | <span data-ttu-id="6a0e7-208">Описание</span><span class="sxs-lookup"><span data-stu-id="6a0e7-208">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a0e7-209">custodians</span><span class="sxs-lookup"><span data-stu-id="6a0e7-209">custodians</span></span>|<span data-ttu-id="6a0e7-210">Коллекция [хранитель](../resources/custodian.md)</span><span class="sxs-lookup"><span data-stu-id="6a0e7-210">[custodian](../resources/custodian.md) collection</span></span>| <span data-ttu-id="6a0e7-211">Сотрудники Организации, которые могут обладать данными, относящимися к обращению.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-211">People in an organization who may possess data relevant to the case.</span></span> |
|<span data-ttu-id="6a0e7-212">ревиевсетс</span><span class="sxs-lookup"><span data-stu-id="6a0e7-212">reviewSets</span></span>|<span data-ttu-id="6a0e7-213">Коллекция [reviewing](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="6a0e7-213">[reviewSet](reviewset.md) collection</span></span>| <span data-ttu-id="6a0e7-214">Коллекция наборов проверки в случае.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-214">Collection of review sets in the case.</span></span> <span data-ttu-id="6a0e7-215">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-215">Read-only.</span></span> <span data-ttu-id="6a0e7-216">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-216">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6a0e7-217">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a0e7-217">JSON representation</span></span>

<span data-ttu-id="6a0e7-218">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a0e7-218">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
 
  ],
  "@odata.type": "microsoft.graph.ediscoveryCase"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "description": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
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
