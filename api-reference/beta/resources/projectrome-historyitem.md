---
title: Тип ресурса historyItem
description: Представляет элемент журнала для действия в приложении. Действия пользователей представляют собой одно назначение в вашем приложении (например, телеПЕРЕДАЧИ, документ или текущую кампанию в видеоигре). Когда пользователь наносит это действие, задействование регистрируется в виде элемента журнала, который указывает время начала и окончания для этого действия. По мере того как пользователь повторно перезапускается с этим действием, для одного действия пользователя записываются несколько элементов журнала.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: c43a4f0515f8d61625e11abe8bbdbe2464c729f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344082"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="a4441-106">Тип ресурса historyItem</span><span class="sxs-lookup"><span data-stu-id="a4441-106">historyItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4441-107">Представляет элемент журнала для [действия](projectrome-activity.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="a4441-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="a4441-108">Действия пользователей представляют собой одно назначение в вашем приложении (например, телеПЕРЕДАЧИ, документ или текущую кампанию в видеоигре).</span><span class="sxs-lookup"><span data-stu-id="a4441-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="a4441-109">Когда пользователь наносит это действие, задействование регистрируется в виде элемента журнала, который указывает время начала и окончания для этого действия.</span><span class="sxs-lookup"><span data-stu-id="a4441-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="a4441-110">По мере того как пользователь повторно перезапускается с этим действием, для одного действия пользователя записываются несколько элементов журнала.</span><span class="sxs-lookup"><span data-stu-id="a4441-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="a4441-111">Когда приложение создает сеанс, объект **historyItem** должен быть добавлен в объект **Activity** для отражения периода участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="a4441-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="a4441-112">Каждый раз, когда пользователь передается с действием, для начисления задействования пользователей добавляется новый **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="a4441-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="a4441-113">Методы</span><span class="sxs-lookup"><span data-stu-id="a4441-113">Methods</span></span>

|<span data-ttu-id="a4441-114">Метод</span><span class="sxs-lookup"><span data-stu-id="a4441-114">Method</span></span> | <span data-ttu-id="a4441-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4441-115">Return Type</span></span> | <span data-ttu-id="a4441-116">Описание</span><span class="sxs-lookup"><span data-stu-id="a4441-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="a4441-117">Создание или замена historyItem</span><span class="sxs-lookup"><span data-stu-id="a4441-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="a4441-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="a4441-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="a4441-119">Создает или заменяет существующий **historyItem** для этого действия (UPSERT).</span><span class="sxs-lookup"><span data-stu-id="a4441-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="a4441-120">Идентификатор должен быть ИДЕНТИФИКАТОРом GUID.</span><span class="sxs-lookup"><span data-stu-id="a4441-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="a4441-121">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="a4441-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="a4441-122">Нет контента</span><span class="sxs-lookup"><span data-stu-id="a4441-122">No Content</span></span> | <span data-ttu-id="a4441-123">Удаляет указанный **historyItem** для этого действия.</span><span class="sxs-lookup"><span data-stu-id="a4441-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4441-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4441-124">Properties</span></span>

|<span data-ttu-id="a4441-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a4441-125">Name</span></span> | <span data-ttu-id="a4441-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a4441-126">Type</span></span> | <span data-ttu-id="a4441-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a4441-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="a4441-128">status</span><span class="sxs-lookup"><span data-stu-id="a4441-128">status</span></span> | <span data-ttu-id="a4441-129">string</span><span class="sxs-lookup"><span data-stu-id="a4441-129">string</span></span> | <span data-ttu-id="a4441-130">ЗаДается сервером.</span><span class="sxs-lookup"><span data-stu-id="a4441-130">Set by the server.</span></span> <span data-ttu-id="a4441-131">Код состояния, используемый для идентификации допустимых объектов.</span><span class="sxs-lookup"><span data-stu-id="a4441-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="a4441-132">Значения: активные, обновленные, удаленные, проигнорированы.</span><span class="sxs-lookup"><span data-stu-id="a4441-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="a4441-133">Усертимезоне</span><span class="sxs-lookup"><span data-stu-id="a4441-133">userTimezone</span></span> | <span data-ttu-id="a4441-134">String</span><span class="sxs-lookup"><span data-stu-id="a4441-134">String</span></span> | <span data-ttu-id="a4441-135">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="a4441-135">Optional.</span></span> <span data-ttu-id="a4441-136">Часовой пояс, в котором устройство пользователя, используемое для создания действия, было размещено во время создания действия.</span><span class="sxs-lookup"><span data-stu-id="a4441-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="a4441-137">Значения, предоставляемые как идентификаторы Олсона для поддержки представления на нескольких платформах.</span><span class="sxs-lookup"><span data-stu-id="a4441-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="a4441-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4441-138">createdDateTime</span></span> | <span data-ttu-id="a4441-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4441-139">DateTimeOffset</span></span> | <span data-ttu-id="a4441-140">ЗаДается сервером.</span><span class="sxs-lookup"><span data-stu-id="a4441-140">Set by the server.</span></span> <span data-ttu-id="a4441-141">Дата и время в формате UTC, когда объект был создан на сервере.</span><span class="sxs-lookup"><span data-stu-id="a4441-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="a4441-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4441-142">lastModifiedDateTime</span></span> | <span data-ttu-id="a4441-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4441-143">DateTimeOffset</span></span> | <span data-ttu-id="a4441-144">ЗаДается сервером.</span><span class="sxs-lookup"><span data-stu-id="a4441-144">Set by the server.</span></span> <span data-ttu-id="a4441-145">Дата и время в формате UTC, когда объект был изменен на сервере.</span><span class="sxs-lookup"><span data-stu-id="a4441-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="a4441-146">id</span><span class="sxs-lookup"><span data-stu-id="a4441-146">id</span></span> | <span data-ttu-id="a4441-147">String</span><span class="sxs-lookup"><span data-stu-id="a4441-147">String</span></span> | <span data-ttu-id="a4441-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4441-148">Required.</span></span> <span data-ttu-id="a4441-149">Идентификатор GUID для объекта **historyItem** в клиентском наборе.</span><span class="sxs-lookup"><span data-stu-id="a4441-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="a4441-150">Стартеддатетиме</span><span class="sxs-lookup"><span data-stu-id="a4441-150">startedDateTime</span></span> | <span data-ttu-id="a4441-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4441-151">DateTimeOffset</span></span> | <span data-ttu-id="a4441-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4441-152">Required.</span></span> <span data-ttu-id="a4441-153">Дата и время (UTC) при запуске **historyItem** (сеанс активности).</span><span class="sxs-lookup"><span data-stu-id="a4441-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="a4441-154">Обязательный для журнала временной шкалы.</span><span class="sxs-lookup"><span data-stu-id="a4441-154">Required for timeline history.</span></span>|
|<span data-ttu-id="a4441-155">Ластактиведатетиме</span><span class="sxs-lookup"><span data-stu-id="a4441-155">lastActiveDateTime</span></span> | <span data-ttu-id="a4441-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4441-156">DateTimeOffset</span></span> | <span data-ttu-id="a4441-157">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="a4441-157">Optional.</span></span> <span data-ttu-id="a4441-158">Дата и время (в формате UTC), когда **historyItem** (сеанс активности) использовался в последний раз как активный или завершенный — если значение равно null, то состояние **HistoryItem** должно быть текущим.</span><span class="sxs-lookup"><span data-stu-id="a4441-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="a4441-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a4441-159">expirationDateTime</span></span> | <span data-ttu-id="a4441-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4441-160">DateTimeOffset</span></span> | <span data-ttu-id="a4441-161">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="a4441-161">Optional.</span></span> <span data-ttu-id="a4441-162">Дата и время в формате UTC, когда **historyItem** будет окончательно удален.</span><span class="sxs-lookup"><span data-stu-id="a4441-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="a4441-163">Может быть задано клиентом.</span><span class="sxs-lookup"><span data-stu-id="a4441-163">Can be set by the client.</span></span>|
|<span data-ttu-id="a4441-164">Активедуратионсекондс</span><span class="sxs-lookup"><span data-stu-id="a4441-164">activeDurationSeconds</span></span> | <span data-ttu-id="a4441-165">int</span><span class="sxs-lookup"><span data-stu-id="a4441-165">int</span></span> | <span data-ttu-id="a4441-166">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a4441-166">Optional.</span></span> <span data-ttu-id="a4441-167">Продолжительность активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="a4441-167">The duration of active user engagement.</span></span> <span data-ttu-id="a4441-168">Если этот параметр не указан, вычисляется из **стартеддатетиме** и **ластактиведатетиме**.</span><span class="sxs-lookup"><span data-stu-id="a4441-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4441-169">Связи</span><span class="sxs-lookup"><span data-stu-id="a4441-169">Relationships</span></span>

|<span data-ttu-id="a4441-170">Отношение</span><span class="sxs-lookup"><span data-stu-id="a4441-170">Relationship</span></span> | <span data-ttu-id="a4441-171">Тип</span><span class="sxs-lookup"><span data-stu-id="a4441-171">Type</span></span> | <span data-ttu-id="a4441-172">Описание</span><span class="sxs-lookup"><span data-stu-id="a4441-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="a4441-173">activity</span><span class="sxs-lookup"><span data-stu-id="a4441-173">activity</span></span>| [<span data-ttu-id="a4441-174">действии</span><span class="sxs-lookup"><span data-stu-id="a4441-174">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="a4441-175">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="a4441-175">Optional.</span></span> <span data-ttu-id="a4441-176">Свойство NavigationProperty/вложение; свойство навигации для связанного действия.</span><span class="sxs-lookup"><span data-stu-id="a4441-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4441-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4441-177">JSON representation</span></span>

<span data-ttu-id="a4441-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4441-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
