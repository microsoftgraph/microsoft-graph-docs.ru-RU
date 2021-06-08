---
title: Тип ресурса timecard
description: Запись в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 25818e091ac2d4f6590fd7ea2c395752d0238bd0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786412"
---
# <a name="timecard-resource-type"></a><span data-ttu-id="668c5-103">Тип ресурса timecard</span><span class="sxs-lookup"><span data-stu-id="668c5-103">timecard resource type</span></span>

<span data-ttu-id="668c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="668c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="668c5-105">Представляет запись химкарта в расписании.</span><span class="sxs-lookup"><span data-stu-id="668c5-105">Represents a timecard entry in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="668c5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="668c5-106">Methods</span></span>

| <span data-ttu-id="668c5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="668c5-107">Method</span></span>       | <span data-ttu-id="668c5-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="668c5-108">Return type</span></span>  |<span data-ttu-id="668c5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="668c5-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="668c5-110">Список</span><span class="sxs-lookup"><span data-stu-id="668c5-110">List</span></span>](../api/timecard-list.md) | <span data-ttu-id="668c5-111">[коллекция timeCard](timecard.md)</span><span class="sxs-lookup"><span data-stu-id="668c5-111">[timeCard](timecard.md) collection</span></span> | <span data-ttu-id="668c5-112">Получите список объектов **timecard** в этом расписании.</span><span class="sxs-lookup"><span data-stu-id="668c5-112">Get the list of **timecard** objects in this schedule.</span></span>|
|[<span data-ttu-id="668c5-113">Создание</span><span class="sxs-lookup"><span data-stu-id="668c5-113">Create</span></span>](../api/timecard-post.md) | [<span data-ttu-id="668c5-114">timeCard</span><span class="sxs-lookup"><span data-stu-id="668c5-114">timeCard</span></span>](timecard.md) | <span data-ttu-id="668c5-115">Создайте новый **объект timecard.**</span><span class="sxs-lookup"><span data-stu-id="668c5-115">Create a new **timecard** object.</span></span>|
|<span data-ttu-id="668c5-116">[получение](../api/timecard-get.md);</span><span class="sxs-lookup"><span data-stu-id="668c5-116">[Get](../api/timecard-get.md)</span></span> | [<span data-ttu-id="668c5-117">timeCard</span><span class="sxs-lookup"><span data-stu-id="668c5-117">timeCard</span></span>](timecard.md) | <span data-ttu-id="668c5-118">Получите **объект timecard** по ID.</span><span class="sxs-lookup"><span data-stu-id="668c5-118">Get a **timecard** object by ID.</span></span>|
|[<span data-ttu-id="668c5-119">Replace</span><span class="sxs-lookup"><span data-stu-id="668c5-119">Replace</span></span>](../api/timecard-replace.md) | <span data-ttu-id="668c5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="668c5-120">None</span></span> | <span data-ttu-id="668c5-121">Замените **объект timecard.**</span><span class="sxs-lookup"><span data-stu-id="668c5-121">Replace a **timecard** object.</span></span>|
|[<span data-ttu-id="668c5-122">Delete</span><span class="sxs-lookup"><span data-stu-id="668c5-122">Delete</span></span>](../api/timecard-delete.md) | <span data-ttu-id="668c5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="668c5-123">None</span></span> | <span data-ttu-id="668c5-124">Удаление объекта **timecard** из расписания.</span><span class="sxs-lookup"><span data-stu-id="668c5-124">Delete a **timecard** object from the schedule.</span></span>|
|[<span data-ttu-id="668c5-125">clockIn</span><span class="sxs-lookup"><span data-stu-id="668c5-125">clockIn</span></span>](../api/timecard-clockin.md) | [<span data-ttu-id="668c5-126">timeCard</span><span class="sxs-lookup"><span data-stu-id="668c5-126">timeCard</span></span>](timecard.md) | <span data-ttu-id="668c5-127">Часы, чтобы запустить **хронограф.**</span><span class="sxs-lookup"><span data-stu-id="668c5-127">Clock in to start a **timecard**.</span></span>|
|[<span data-ttu-id="668c5-128">clockOut</span><span class="sxs-lookup"><span data-stu-id="668c5-128">clockOut</span></span>](../api/timecard-clockout.md) | <span data-ttu-id="668c5-129">Нет</span><span class="sxs-lookup"><span data-stu-id="668c5-129">None</span></span> | <span data-ttu-id="668c5-130">Часы, чтобы положить конец **открытой карточке времени**.</span><span class="sxs-lookup"><span data-stu-id="668c5-130">Clock out to end an open **timecard**.</span></span>|
|[<span data-ttu-id="668c5-131">startBreak</span><span class="sxs-lookup"><span data-stu-id="668c5-131">startBreak</span></span>](../api/timecard-startbreak.md) | <span data-ttu-id="668c5-132">Нет</span><span class="sxs-lookup"><span data-stu-id="668c5-132">None</span></span> | <span data-ttu-id="668c5-133">Запустите **timeCardBreak** в определенной **карточке времени.**</span><span class="sxs-lookup"><span data-stu-id="668c5-133">Start a **timeCardBreak** in a specific **timecard**.</span></span>|
|[<span data-ttu-id="668c5-134">endBreak</span><span class="sxs-lookup"><span data-stu-id="668c5-134">endBreak</span></span>](../api/timecard-endbreak.md) | <span data-ttu-id="668c5-135">Нет</span><span class="sxs-lookup"><span data-stu-id="668c5-135">None</span></span> | <span data-ttu-id="668c5-136">Завершение открытого **времениCardBreak** в определенной **карточке времени.**</span><span class="sxs-lookup"><span data-stu-id="668c5-136">End the open **timeCardBreak** in a specific **timecard**.</span></span>|
|[<span data-ttu-id="668c5-137">confirmTimeCard</span><span class="sxs-lookup"><span data-stu-id="668c5-137">confirmTimeCard</span></span>](../api/timecard-confirm.md) | <span data-ttu-id="668c5-138">Нет</span><span class="sxs-lookup"><span data-stu-id="668c5-138">None</span></span> | <span data-ttu-id="668c5-139">Подтверждение **записи химкарта.**</span><span class="sxs-lookup"><span data-stu-id="668c5-139">Confirm a **timecard** record.</span></span>|

## <a name="properties"></a><span data-ttu-id="668c5-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="668c5-140">Properties</span></span>
|<span data-ttu-id="668c5-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="668c5-141">Property</span></span>               |<span data-ttu-id="668c5-142">Тип</span><span class="sxs-lookup"><span data-stu-id="668c5-142">Type</span></span>           |<span data-ttu-id="668c5-143">Описание</span><span class="sxs-lookup"><span data-stu-id="668c5-143">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="668c5-144">id</span><span class="sxs-lookup"><span data-stu-id="668c5-144">id</span></span>                    |`string`  |<span data-ttu-id="668c5-145">ID **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="668c5-145">ID of the **timeCard**.</span></span>|
| <span data-ttu-id="668c5-146">userId</span><span class="sxs-lookup"><span data-stu-id="668c5-146">userId</span></span>                    |`string` |<span data-ttu-id="668c5-147">Пользовательский ID, к которому **принадлежит timeCard.**</span><span class="sxs-lookup"><span data-stu-id="668c5-147">User ID to which  the **timeCard** belongs.</span></span> |
| <span data-ttu-id="668c5-148">state</span><span class="sxs-lookup"><span data-stu-id="668c5-148">state</span></span>                 |`timeCardState`  | <span data-ttu-id="668c5-149">Текущее состояние **timeCard во** время жизненного цикла. Возможные значения: `clockedIn` `onBreak` , , `clockedOut` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="668c5-149">The current state of the **timeCard** during its life cycle.Possible values are: `clockedIn`, `onBreak`, `clockedOut`, `unknownFutureValue`.</span></span>|
| <span data-ttu-id="668c5-150">clockInEvent</span><span class="sxs-lookup"><span data-stu-id="668c5-150">clockInEvent</span></span>       |[<span data-ttu-id="668c5-151">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="668c5-151">timeCardEvent</span></span>](../resources/timecardevent.md)    | <span data-ttu-id="668c5-152">Событие с часовой стрелкой **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="668c5-152">The clock-in event of the **timeCard**.</span></span> |
| <span data-ttu-id="668c5-153">clockOutEvent</span><span class="sxs-lookup"><span data-stu-id="668c5-153">clockOutEvent</span></span>                 |[<span data-ttu-id="668c5-154">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="668c5-154">timeCardEvent</span></span>](../resources/timecardevent.md)  |<span data-ttu-id="668c5-155">Событие clock-out **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="668c5-155">The clock-out event of the **timeCard**.</span></span> |
| <span data-ttu-id="668c5-156">notes</span><span class="sxs-lookup"><span data-stu-id="668c5-156">notes</span></span>                 | [<span data-ttu-id="668c5-157">itemBody</span><span class="sxs-lookup"><span data-stu-id="668c5-157">itemBody</span></span>](itembody.md)  |<span data-ttu-id="668c5-158">Заметки о **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="668c5-158">Notes about the **timeCard**.</span></span> |
| <span data-ttu-id="668c5-159">перерывы</span><span class="sxs-lookup"><span data-stu-id="668c5-159">breaks</span></span>    |<span data-ttu-id="668c5-160">[коллекция timeCardBreak](timecardbreak.md)</span><span class="sxs-lookup"><span data-stu-id="668c5-160">[timeCardBreak](timecardbreak.md) collection</span></span>  |<span data-ttu-id="668c5-161">Список перерывов, связанных с **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="668c5-161">The list of breaks associated with the **timeCard**.</span></span>|
| <span data-ttu-id="668c5-162">originalEntry</span><span class="sxs-lookup"><span data-stu-id="668c5-162">originalEntry</span></span>| [<span data-ttu-id="668c5-163">timeCardEntry</span><span class="sxs-lookup"><span data-stu-id="668c5-163">timeCardEntry</span></span>](../resources/timecardentry.md) | <span data-ttu-id="668c5-164">Исходное **времяCardEntry** **timeCard** перед изменением пользователя.</span><span class="sxs-lookup"><span data-stu-id="668c5-164">The original **timeCardEntry** of the **timeCard**, before user edits.</span></span> |
| <span data-ttu-id="668c5-165">confirmedBy</span><span class="sxs-lookup"><span data-stu-id="668c5-165">confirmedBy</span></span> |`confirmedBy`    | <span data-ttu-id="668c5-166">Указать, подтверждена ли эта запись **timeCard.**</span><span class="sxs-lookup"><span data-stu-id="668c5-166">Indicate if this **timeCard** entry is confirmed.</span></span> <span data-ttu-id="668c5-167">Возможные значения: `none`, `user`, `manager`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="668c5-167">Possible values are `none`, `user`, `manager`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="668c5-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="668c5-168">createdDateTime</span></span>|`Edm.dateTimeOffset`| <span data-ttu-id="668c5-169">Время создания **timeCard.**</span><span class="sxs-lookup"><span data-stu-id="668c5-169">The timestamp in which the **timeCard** was created.</span></span> |
|<span data-ttu-id="668c5-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="668c5-170">createdBy</span></span>|`IdentitySet`| <span data-ttu-id="668c5-171">Удостоверение лица, создавшего объект.</span><span class="sxs-lookup"><span data-stu-id="668c5-171">Identity of the person who created the entity.</span></span> |
|<span data-ttu-id="668c5-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="668c5-172">lastModifiedDateTime</span></span>|`dateTimeOffset`| <span data-ttu-id="668c5-173">Время последнего изменения **timeCard.**</span><span class="sxs-lookup"><span data-stu-id="668c5-173">The timestamp in which the **timeCard** was last modified.</span></span>|
|<span data-ttu-id="668c5-174">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="668c5-174">lastModifiedBy</span></span>| `IdentitySet`| <span data-ttu-id="668c5-175">Удостоверение человека, который в последний раз изменил объект.</span><span class="sxs-lookup"><span data-stu-id="668c5-175">Identity of the person who last modified the entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="668c5-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="668c5-176">JSON representation</span></span>

<span data-ttu-id="668c5-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="668c5-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCard",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "clockInEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "clockOutEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "notes" : {"@odata.type":"microsoft.graph.itemBody"},
  "breaks" : [{"@odata.type":"microsoft.graph.timeCardEvent"}],
  "originalEntry" : {"@odata.type":"microsoft.graph.timeCardEntry"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCard resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
