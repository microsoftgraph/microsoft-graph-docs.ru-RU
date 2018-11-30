---
title: Тип ресурса historyItem
description: Представляет элемент журнала для действия в приложении. Действия пользователя представляют одну целевую в вашем приложении -, например Показать TV, документа или текущей кампании в игру. Когда пользователь подключает с помощью этого действия, деловые регистрируются как элемента журнала, которое указывает время начала и окончания для этого действия. Как пользователь повторно массовых с этой операции со временем, несколько элементов журнала записываются действия одного пользователя.
ms.openlocfilehash: f413da4280f7b39f0be2a9dafd872ebee041ccc8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027064"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="dc1b1-106">Тип ресурса historyItem</span><span class="sxs-lookup"><span data-stu-id="dc1b1-106">historyItem resource type</span></span>

<span data-ttu-id="dc1b1-107">Представляет элемент журнала для [действия](projectrome-activity.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="dc1b1-108">Действия пользователя представляют одну целевую в вашем приложении -, например Показать TV, документа или текущей кампании в игру.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="dc1b1-109">Когда пользователь подключает с помощью этого действия, деловые регистрируются как элемента журнала, которое указывает время начала и окончания для этого действия.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="dc1b1-110">Как пользователь повторно массовых с этой операции со временем, несколько элементов журнала записываются действия одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="dc1b1-111">Когда приложение создает сеанс, объект **historyItem** следует добавить объект **активности** в соответствии с период участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="dc1b1-112">Каждый раз, пользователь снова подключает с действием, новые **historyItem** добавляется активности начисления участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="dc1b1-113">Методы</span><span class="sxs-lookup"><span data-stu-id="dc1b1-113">Methods</span></span>

|<span data-ttu-id="dc1b1-114">Метод</span><span class="sxs-lookup"><span data-stu-id="dc1b1-114">Method</span></span> | <span data-ttu-id="dc1b1-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc1b1-115">Return Type</span></span> | <span data-ttu-id="dc1b1-116">Описание</span><span class="sxs-lookup"><span data-stu-id="dc1b1-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="dc1b1-117">Создать или заменить historyItem</span><span class="sxs-lookup"><span data-stu-id="dc1b1-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="dc1b1-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="dc1b1-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="dc1b1-119">Создает или заменяет существующий **historyItem** для этого действия (upsert).</span><span class="sxs-lookup"><span data-stu-id="dc1b1-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="dc1b1-120">Идентификатор должен быть идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="dc1b1-121">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="dc1b1-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="dc1b1-122">Нет содержимого</span><span class="sxs-lookup"><span data-stu-id="dc1b1-122">No Content</span></span> | <span data-ttu-id="dc1b1-123">Удаляет указанный **historyItem** для этого действия.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc1b1-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc1b1-124">Properties</span></span>

|<span data-ttu-id="dc1b1-125">Имя</span><span class="sxs-lookup"><span data-stu-id="dc1b1-125">Name</span></span> | <span data-ttu-id="dc1b1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="dc1b1-126">Type</span></span> | <span data-ttu-id="dc1b1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="dc1b1-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="dc1b1-128">status</span><span class="sxs-lookup"><span data-stu-id="dc1b1-128">status</span></span> | <span data-ttu-id="dc1b1-129">status</span><span class="sxs-lookup"><span data-stu-id="dc1b1-129">status</span></span> | <span data-ttu-id="dc1b1-130">Установка с сервера.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-130">Set by the server.</span></span> <span data-ttu-id="dc1b1-131">Код состояния, используемое для идентификации допустимый объекты.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="dc1b1-132">Значения: активный, обновления, удаления, игнорируются.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="dc1b1-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="dc1b1-133">userTimezone</span></span> | <span data-ttu-id="dc1b1-134">String</span><span class="sxs-lookup"><span data-stu-id="dc1b1-134">String</span></span> | <span data-ttu-id="dc1b1-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-135">Optional.</span></span> <span data-ttu-id="dc1b1-136">Часовой пояс, в котором устройством пользователя, используемый для создания операции находился во время создания активности.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="dc1b1-137">Значения, указанные как Олсон идентификаторы для поддержки различных платформах представление.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="dc1b1-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1b1-138">createdDateTime</span></span> | <span data-ttu-id="dc1b1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1b1-139">DateTimeOffset</span></span> | <span data-ttu-id="dc1b1-140">Установка с сервера.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-140">Set by the server.</span></span> <span data-ttu-id="dc1b1-141">Дата и время в формате UTC, когда объект был создан на сервере.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="dc1b1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1b1-142">lastModifiedDateTime</span></span> | <span data-ttu-id="dc1b1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1b1-143">DateTimeOffset</span></span> | <span data-ttu-id="dc1b1-144">Установка с сервера.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-144">Set by the server.</span></span> <span data-ttu-id="dc1b1-145">Дата и время в формате UTC, когда объект был изменен на сервере.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="dc1b1-146">id</span><span class="sxs-lookup"><span data-stu-id="dc1b1-146">id</span></span> | <span data-ttu-id="dc1b1-147">Строка</span><span class="sxs-lookup"><span data-stu-id="dc1b1-147">String</span></span> | <span data-ttu-id="dc1b1-148">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-148">Required.</span></span> <span data-ttu-id="dc1b1-149">Идентификатор GUID набора клиента для объекта **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="dc1b1-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="dc1b1-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1b1-150">startedDateTime</span></span> | <span data-ttu-id="dc1b1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1b1-151">DateTimeOffset</span></span> | <span data-ttu-id="dc1b1-152">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-152">Required.</span></span> <span data-ttu-id="dc1b1-153">При запуске **historyItem** (активности сеанса) UTC даты и времени.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="dc1b1-154">Требуется для журнал временной шкалы.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-154">Required for timeline history.</span></span>|
|<span data-ttu-id="dc1b1-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1b1-155">lastActiveDateTime</span></span> | <span data-ttu-id="dc1b1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1b1-156">DateTimeOffset</span></span> | <span data-ttu-id="dc1b1-157">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-157">Optional.</span></span> <span data-ttu-id="dc1b1-158">При **historyItem** (активности сеанса) последнего был распознан как активных, так и по завершении работы — Если значение null, **historyItem** состояние UTC даты и времени должны быть Ongoing.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="dc1b1-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1b1-159">expirationDateTime</span></span> | <span data-ttu-id="dc1b1-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1b1-160">DateTimeOffset</span></span> | <span data-ttu-id="dc1b1-161">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-161">Optional.</span></span> <span data-ttu-id="dc1b1-162">Даты-времени UTC при **historyItem** подвергнется окончательного удаления.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="dc1b1-163">Можно задать клиентом.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-163">Can be set by the client.</span></span>|
|<span data-ttu-id="dc1b1-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="dc1b1-164">activeDurationSeconds</span></span> | <span data-ttu-id="dc1b1-165">целое</span><span class="sxs-lookup"><span data-stu-id="dc1b1-165">int</span></span> | <span data-ttu-id="dc1b1-166">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-166">Optional.</span></span> <span data-ttu-id="dc1b1-167">Продолжительность сотрудничества активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-167">The duration of active user engagement.</span></span> <span data-ttu-id="dc1b1-168">Если не указано, отсчитывается от **startedDateTime** и **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc1b1-169">Связи</span><span class="sxs-lookup"><span data-stu-id="dc1b1-169">Relationships</span></span>

|<span data-ttu-id="dc1b1-170">Связь</span><span class="sxs-lookup"><span data-stu-id="dc1b1-170">Relationship</span></span> | <span data-ttu-id="dc1b1-171">Тип</span><span class="sxs-lookup"><span data-stu-id="dc1b1-171">Type</span></span> | <span data-ttu-id="dc1b1-172">Description</span><span class="sxs-lookup"><span data-stu-id="dc1b1-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="dc1b1-173">activity</span><span class="sxs-lookup"><span data-stu-id="dc1b1-173">activity</span></span>| [<span data-ttu-id="dc1b1-174">userActivity</span><span class="sxs-lookup"><span data-stu-id="dc1b1-174">userActivity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="dc1b1-175">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-175">Optional.</span></span> <span data-ttu-id="dc1b1-176">NavigationProperty/вложенности; свойство навигации для связанного действия.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc1b1-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc1b1-177">JSON representation</span></span>

<span data-ttu-id="dc1b1-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc1b1-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
