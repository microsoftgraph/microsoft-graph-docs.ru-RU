---
title: Тип ресурса historyItem
description: Представляет элемент журнала для действия в приложении. Действия пользователей представляют собой одно назначение в вашем приложении (например, телепередачи, документ или текущую кампанию в видеоигре). Когда пользователь наносит это действие, задействование регистрируется в виде элемента журнала, который указывает время начала и окончания для этого действия. По мере того как пользователь повторно перезапускается с этим действием, для одного действия пользователя записываются несколько элементов журнала.
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ''
ms.openlocfilehash: cd83657c99b4fb2e5ce077549d51d60329ae9d60
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521420"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="bafca-106">Тип ресурса historyItem</span><span class="sxs-lookup"><span data-stu-id="bafca-106">historyItem resource type</span></span>

<span data-ttu-id="bafca-107">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bafca-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bafca-108">Представляет элемент журнала для [действия](projectrome-activity.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="bafca-108">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="bafca-109">Действия пользователей представляют собой одно назначение в вашем приложении (например, телепередачи, документ или текущую кампанию в видеоигре).</span><span class="sxs-lookup"><span data-stu-id="bafca-109">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="bafca-110">Когда пользователь наносит это действие, задействование регистрируется в виде элемента журнала, который указывает время начала и окончания для этого действия.</span><span class="sxs-lookup"><span data-stu-id="bafca-110">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="bafca-111">По мере того как пользователь повторно перезапускается с этим действием, для одного действия пользователя записываются несколько элементов журнала.</span><span class="sxs-lookup"><span data-stu-id="bafca-111">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="bafca-112">Когда приложение создает сеанс, объект **historyItem** должен быть добавлен в объект **Activity** для отражения периода участия пользователя.</span><span class="sxs-lookup"><span data-stu-id="bafca-112">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="bafca-113">Каждый раз, когда пользователь передается с действием, для начисления задействования пользователей добавляется новый **historyItem** .</span><span class="sxs-lookup"><span data-stu-id="bafca-113">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="bafca-114">Методы</span><span class="sxs-lookup"><span data-stu-id="bafca-114">Methods</span></span>

|<span data-ttu-id="bafca-115">Метод</span><span class="sxs-lookup"><span data-stu-id="bafca-115">Method</span></span> | <span data-ttu-id="bafca-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bafca-116">Return Type</span></span> | <span data-ttu-id="bafca-117">Описание</span><span class="sxs-lookup"><span data-stu-id="bafca-117">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="bafca-118">Создание или замена historyItem</span><span class="sxs-lookup"><span data-stu-id="bafca-118">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="bafca-119">historyItem</span><span class="sxs-lookup"><span data-stu-id="bafca-119">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="bafca-120">Создает или заменяет существующий **historyItem** для этого действия (UPSERT).</span><span class="sxs-lookup"><span data-stu-id="bafca-120">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="bafca-121">Идентификатор должен быть идентификатором GUID.</span><span class="sxs-lookup"><span data-stu-id="bafca-121">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="bafca-122">Удаление historyItem</span><span class="sxs-lookup"><span data-stu-id="bafca-122">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="bafca-123">Содержимое отсутствует</span><span class="sxs-lookup"><span data-stu-id="bafca-123">No Content</span></span> | <span data-ttu-id="bafca-124">Удаляет указанный **historyItem** для этого действия.</span><span class="sxs-lookup"><span data-stu-id="bafca-124">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="bafca-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="bafca-125">Properties</span></span>

|<span data-ttu-id="bafca-126">Имя</span><span class="sxs-lookup"><span data-stu-id="bafca-126">Name</span></span> | <span data-ttu-id="bafca-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bafca-127">Type</span></span> | <span data-ttu-id="bafca-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bafca-128">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="bafca-129">status</span><span class="sxs-lookup"><span data-stu-id="bafca-129">status</span></span> | <span data-ttu-id="bafca-130">string</span><span class="sxs-lookup"><span data-stu-id="bafca-130">string</span></span> | <span data-ttu-id="bafca-131">Задается сервером.</span><span class="sxs-lookup"><span data-stu-id="bafca-131">Set by the server.</span></span> <span data-ttu-id="bafca-132">Код состояния, используемый для идентификации допустимых объектов.</span><span class="sxs-lookup"><span data-stu-id="bafca-132">A status code used to identify valid objects.</span></span> <span data-ttu-id="bafca-133">Значения: активные, обновленные, удаленные, проигнорированы.</span><span class="sxs-lookup"><span data-stu-id="bafca-133">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="bafca-134">усертимезоне</span><span class="sxs-lookup"><span data-stu-id="bafca-134">userTimezone</span></span> | <span data-ttu-id="bafca-135">String</span><span class="sxs-lookup"><span data-stu-id="bafca-135">String</span></span> | <span data-ttu-id="bafca-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bafca-136">Optional.</span></span> <span data-ttu-id="bafca-137">Часовой пояс, в котором устройство пользователя, используемое для создания действия, было размещено во время создания действия.</span><span class="sxs-lookup"><span data-stu-id="bafca-137">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="bafca-138">Значения, предоставляемые как идентификаторы Олсона для поддержки представления на нескольких платформах.</span><span class="sxs-lookup"><span data-stu-id="bafca-138">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="bafca-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bafca-139">createdDateTime</span></span> | <span data-ttu-id="bafca-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafca-140">DateTimeOffset</span></span> | <span data-ttu-id="bafca-141">Задается сервером.</span><span class="sxs-lookup"><span data-stu-id="bafca-141">Set by the server.</span></span> <span data-ttu-id="bafca-142">Дата и время в формате UTC, когда объект был создан на сервере.</span><span class="sxs-lookup"><span data-stu-id="bafca-142">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="bafca-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bafca-143">lastModifiedDateTime</span></span> | <span data-ttu-id="bafca-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafca-144">DateTimeOffset</span></span> | <span data-ttu-id="bafca-145">Задается сервером.</span><span class="sxs-lookup"><span data-stu-id="bafca-145">Set by the server.</span></span> <span data-ttu-id="bafca-146">Дата и время в формате UTC, когда объект был изменен на сервере.</span><span class="sxs-lookup"><span data-stu-id="bafca-146">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="bafca-147">id</span><span class="sxs-lookup"><span data-stu-id="bafca-147">id</span></span> | <span data-ttu-id="bafca-148">String</span><span class="sxs-lookup"><span data-stu-id="bafca-148">String</span></span> | <span data-ttu-id="bafca-149">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bafca-149">Required.</span></span> <span data-ttu-id="bafca-150">Идентификатор GUID для объекта **historyItem** в клиентском наборе.</span><span class="sxs-lookup"><span data-stu-id="bafca-150">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="bafca-151">стартеддатетиме</span><span class="sxs-lookup"><span data-stu-id="bafca-151">startedDateTime</span></span> | <span data-ttu-id="bafca-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafca-152">DateTimeOffset</span></span> | <span data-ttu-id="bafca-153">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="bafca-153">Required.</span></span> <span data-ttu-id="bafca-154">Дата и время (UTC) при запуске **historyItem** (сеанс активности).</span><span class="sxs-lookup"><span data-stu-id="bafca-154">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="bafca-155">Обязательный для журнала временной шкалы.</span><span class="sxs-lookup"><span data-stu-id="bafca-155">Required for timeline history.</span></span>|
|<span data-ttu-id="bafca-156">ластактиведатетиме</span><span class="sxs-lookup"><span data-stu-id="bafca-156">lastActiveDateTime</span></span> | <span data-ttu-id="bafca-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafca-157">DateTimeOffset</span></span> | <span data-ttu-id="bafca-158">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="bafca-158">Optional.</span></span> <span data-ttu-id="bafca-159">Дата и время (в формате UTC), когда **historyItem** (сеанс активности) использовался в последний раз как активный или завершенный — если значение равно null, то состояние **HistoryItem** должно быть текущим.</span><span class="sxs-lookup"><span data-stu-id="bafca-159">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="bafca-160">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bafca-160">expirationDateTime</span></span> | <span data-ttu-id="bafca-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bafca-161">DateTimeOffset</span></span> | <span data-ttu-id="bafca-162">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="bafca-162">Optional.</span></span> <span data-ttu-id="bafca-163">Дата и время в формате UTC, когда **historyItem** будет окончательно удален.</span><span class="sxs-lookup"><span data-stu-id="bafca-163">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="bafca-164">Может быть задано клиентом.</span><span class="sxs-lookup"><span data-stu-id="bafca-164">Can be set by the client.</span></span>|
|<span data-ttu-id="bafca-165">активедуратионсекондс</span><span class="sxs-lookup"><span data-stu-id="bafca-165">activeDurationSeconds</span></span> | <span data-ttu-id="bafca-166">int</span><span class="sxs-lookup"><span data-stu-id="bafca-166">int</span></span> | <span data-ttu-id="bafca-167">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bafca-167">Optional.</span></span> <span data-ttu-id="bafca-168">Продолжительность активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="bafca-168">The duration of active user engagement.</span></span> <span data-ttu-id="bafca-169">Если этот параметр не указан, вычисляется из **стартеддатетиме** и **ластактиведатетиме**.</span><span class="sxs-lookup"><span data-stu-id="bafca-169">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bafca-170">Связи</span><span class="sxs-lookup"><span data-stu-id="bafca-170">Relationships</span></span>

|<span data-ttu-id="bafca-171">Связь</span><span class="sxs-lookup"><span data-stu-id="bafca-171">Relationship</span></span> | <span data-ttu-id="bafca-172">Тип</span><span class="sxs-lookup"><span data-stu-id="bafca-172">Type</span></span> | <span data-ttu-id="bafca-173">Описание</span><span class="sxs-lookup"><span data-stu-id="bafca-173">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="bafca-174">activity</span><span class="sxs-lookup"><span data-stu-id="bafca-174">activity</span></span>| [<span data-ttu-id="bafca-175">действии</span><span class="sxs-lookup"><span data-stu-id="bafca-175">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="bafca-176">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="bafca-176">Optional.</span></span> <span data-ttu-id="bafca-177">Свойство NavigationProperty/вложение; свойство навигации для связанного действия.</span><span class="sxs-lookup"><span data-stu-id="bafca-177">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bafca-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bafca-178">JSON representation</span></span>

<span data-ttu-id="bafca-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bafca-179">Here is a JSON representation of the resource.</span></span>

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
