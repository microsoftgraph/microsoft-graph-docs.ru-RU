---
title: Тип ресурса historyItem
description: Представляет элемент журнала для действия в приложении. Действия пользователя представляют одну целевую в вашем приложении -, например Показать TV, документа или текущей кампании в игру. Когда пользователь подключает с помощью этого действия, деловые регистрируются как элемента журнала, которое указывает время начала и окончания для этого действия. Как пользователь повторно массовых с этой операции со временем, несколько элементов журнала записываются действия одного пользователя.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 168587aa54446aeee78107deaa9087c6bffb8586
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976956"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="22d3d-106">Тип ресурса historyItem</span><span class="sxs-lookup"><span data-stu-id="22d3d-106">historyItem resource type</span></span>

> <span data-ttu-id="22d3d-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22d3d-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22d3d-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d3d-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22d3d-109">Представляет элемент журнала для [действия](projectrome-activity.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="22d3d-109">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="22d3d-110">Действия пользователя представляют одну целевую в вашем приложении -, например Показать TV, документа или текущей кампании в игру.</span><span class="sxs-lookup"><span data-stu-id="22d3d-110">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="22d3d-111">Когда пользователь подключает с помощью этого действия, деловые регистрируются как элемента журнала, которое указывает время начала и окончания для этого действия.</span><span class="sxs-lookup"><span data-stu-id="22d3d-111">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="22d3d-112">Как пользователь повторно массовых с этой операции со временем, несколько элементов журнала записываются действия одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="22d3d-112">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="22d3d-113">Когда приложение создает сеанс, объект **historyItem** следует добавить объект **активности** в соответствии с период участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="22d3d-113">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="22d3d-114">Каждый раз, пользователь снова подключает с действием, новые **historyItem** добавляется активности начисления участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="22d3d-114">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="22d3d-115">Методы</span><span class="sxs-lookup"><span data-stu-id="22d3d-115">Methods</span></span>

|<span data-ttu-id="22d3d-116">Метод</span><span class="sxs-lookup"><span data-stu-id="22d3d-116">Method</span></span> | <span data-ttu-id="22d3d-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="22d3d-117">Return Type</span></span> | <span data-ttu-id="22d3d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="22d3d-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="22d3d-119">Создать или заменить historyItem</span><span class="sxs-lookup"><span data-stu-id="22d3d-119">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="22d3d-120">historyItem</span><span class="sxs-lookup"><span data-stu-id="22d3d-120">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="22d3d-121">Создает или заменяет существующий **historyItem** для этого действия (upsert).</span><span class="sxs-lookup"><span data-stu-id="22d3d-121">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="22d3d-122">Идентификатор должен быть идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="22d3d-122">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="22d3d-123">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="22d3d-123">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="22d3d-124">Нет содержимого</span><span class="sxs-lookup"><span data-stu-id="22d3d-124">No Content</span></span> | <span data-ttu-id="22d3d-125">Удаляет указанный **historyItem** для этого действия.</span><span class="sxs-lookup"><span data-stu-id="22d3d-125">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="22d3d-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="22d3d-126">Properties</span></span>

|<span data-ttu-id="22d3d-127">Имя</span><span class="sxs-lookup"><span data-stu-id="22d3d-127">Name</span></span> | <span data-ttu-id="22d3d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="22d3d-128">Type</span></span> | <span data-ttu-id="22d3d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="22d3d-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="22d3d-130">status</span><span class="sxs-lookup"><span data-stu-id="22d3d-130">status</span></span> | <span data-ttu-id="22d3d-131">EnumType</span><span class="sxs-lookup"><span data-stu-id="22d3d-131">EnumType</span></span> | <span data-ttu-id="22d3d-132">Установка с сервера.</span><span class="sxs-lookup"><span data-stu-id="22d3d-132">Set by the server.</span></span> <span data-ttu-id="22d3d-133">Код состояния, используемое для идентификации допустимый объекты.</span><span class="sxs-lookup"><span data-stu-id="22d3d-133">A status code used to identify valid objects.</span></span> <span data-ttu-id="22d3d-134">Значения: активный, обновления, удаления, игнорируются.</span><span class="sxs-lookup"><span data-stu-id="22d3d-134">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="22d3d-135">userTimezone</span><span class="sxs-lookup"><span data-stu-id="22d3d-135">userTimezone</span></span> | <span data-ttu-id="22d3d-136">Строка</span><span class="sxs-lookup"><span data-stu-id="22d3d-136">String</span></span> | <span data-ttu-id="22d3d-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="22d3d-137">Optional.</span></span> <span data-ttu-id="22d3d-138">Часовой пояс, в котором устройством пользователя, используемый для создания операции находился во время создания активности.</span><span class="sxs-lookup"><span data-stu-id="22d3d-138">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="22d3d-139">Значения, указанные как Олсон идентификаторы для поддержки различных платформах представление.</span><span class="sxs-lookup"><span data-stu-id="22d3d-139">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="22d3d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22d3d-140">createdDateTime</span></span> | <span data-ttu-id="22d3d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d3d-141">DateTimeOffset</span></span> | <span data-ttu-id="22d3d-142">Установка с сервера.</span><span class="sxs-lookup"><span data-stu-id="22d3d-142">Set by the server.</span></span> <span data-ttu-id="22d3d-143">Дата и время в формате UTC, когда объект был создан на сервере.</span><span class="sxs-lookup"><span data-stu-id="22d3d-143">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="22d3d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22d3d-144">lastModifiedDateTime</span></span> | <span data-ttu-id="22d3d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d3d-145">DateTimeOffset</span></span> | <span data-ttu-id="22d3d-146">Установка с сервера.</span><span class="sxs-lookup"><span data-stu-id="22d3d-146">Set by the server.</span></span> <span data-ttu-id="22d3d-147">Дата и время в формате UTC, когда объект был изменен на сервере.</span><span class="sxs-lookup"><span data-stu-id="22d3d-147">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="22d3d-148">id</span><span class="sxs-lookup"><span data-stu-id="22d3d-148">id</span></span> | <span data-ttu-id="22d3d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="22d3d-149">String</span></span> | <span data-ttu-id="22d3d-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d3d-150">Required.</span></span> <span data-ttu-id="22d3d-151">Идентификатор GUID набора клиента для объекта **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="22d3d-151">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="22d3d-152">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="22d3d-152">startedDateTime</span></span> | <span data-ttu-id="22d3d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d3d-153">DateTimeOffset</span></span> | <span data-ttu-id="22d3d-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d3d-154">Required.</span></span> <span data-ttu-id="22d3d-155">При запуске **historyItem** (активности сеанса) UTC даты и времени.</span><span class="sxs-lookup"><span data-stu-id="22d3d-155">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="22d3d-156">Требуется для журнал временной шкалы.</span><span class="sxs-lookup"><span data-stu-id="22d3d-156">Required for timeline history.</span></span>|
|<span data-ttu-id="22d3d-157">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="22d3d-157">lastActiveDateTime</span></span> | <span data-ttu-id="22d3d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d3d-158">DateTimeOffset</span></span> | <span data-ttu-id="22d3d-159">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="22d3d-159">Optional.</span></span> <span data-ttu-id="22d3d-160">При **historyItem** (активности сеанса) последнего был распознан как активных, так и по завершении работы — Если значение null, **historyItem** состояние UTC даты и времени должны быть Ongoing.</span><span class="sxs-lookup"><span data-stu-id="22d3d-160">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="22d3d-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="22d3d-161">expirationDateTime</span></span> | <span data-ttu-id="22d3d-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d3d-162">DateTimeOffset</span></span> | <span data-ttu-id="22d3d-163">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="22d3d-163">Optional.</span></span> <span data-ttu-id="22d3d-164">Даты-времени UTC при **historyItem** подвергнется окончательного удаления.</span><span class="sxs-lookup"><span data-stu-id="22d3d-164">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="22d3d-165">Можно задать клиентом.</span><span class="sxs-lookup"><span data-stu-id="22d3d-165">Can be set by the client.</span></span>|
|<span data-ttu-id="22d3d-166">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="22d3d-166">activeDurationSeconds</span></span> | <span data-ttu-id="22d3d-167">int</span><span class="sxs-lookup"><span data-stu-id="22d3d-167">int</span></span> | <span data-ttu-id="22d3d-168">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="22d3d-168">Optional.</span></span> <span data-ttu-id="22d3d-169">Продолжительность сотрудничества активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="22d3d-169">The duration of active user engagement.</span></span> <span data-ttu-id="22d3d-170">Если не указано, отсчитывается от **startedDateTime** и **lastActiveDateTime**.</span><span class="sxs-lookup"><span data-stu-id="22d3d-170">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22d3d-171">Связи</span><span class="sxs-lookup"><span data-stu-id="22d3d-171">Relationships</span></span>

|<span data-ttu-id="22d3d-172">Связь</span><span class="sxs-lookup"><span data-stu-id="22d3d-172">Relationship</span></span> | <span data-ttu-id="22d3d-173">Тип</span><span class="sxs-lookup"><span data-stu-id="22d3d-173">Type</span></span> | <span data-ttu-id="22d3d-174">Описание</span><span class="sxs-lookup"><span data-stu-id="22d3d-174">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="22d3d-175">activity</span><span class="sxs-lookup"><span data-stu-id="22d3d-175">activity</span></span>| [<span data-ttu-id="22d3d-176">действии</span><span class="sxs-lookup"><span data-stu-id="22d3d-176">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="22d3d-177">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="22d3d-177">Optional.</span></span> <span data-ttu-id="22d3d-178">NavigationProperty/вложенности; свойство навигации для связанного действия.</span><span class="sxs-lookup"><span data-stu-id="22d3d-178">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22d3d-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22d3d-179">JSON representation</span></span>

<span data-ttu-id="22d3d-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22d3d-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
