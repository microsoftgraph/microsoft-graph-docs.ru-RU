---
title: Тип ресурса Акцессревиевинстанце
description: Представляет повторение объекта `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 480774950e2257b7af099c02cbe7c6571c0ce4c6
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001070"
---
# <a name="accessreviewinstance-resource-type"></a><span data-ttu-id="da964-103">Тип ресурса Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="da964-103">accessReviewInstance resource type</span></span>

<span data-ttu-id="da964-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da964-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da964-105">Представляет повторение [проверки доступа](accessreviewsv2-root.md) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da964-105">Represents an Azure AD [access review](accessreviewsv2-root.md) recurrence.</span></span> <span data-ttu-id="da964-106">Если родительская [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md) — это повторяющаяся проверка доступа, экземпляры представляют каждое повторение.</span><span class="sxs-lookup"><span data-stu-id="da964-106">If the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="da964-107">Проверка, которая не повторяется, будет иметь ровно один экземпляр.</span><span class="sxs-lookup"><span data-stu-id="da964-107">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="da964-108">Экземпляры также представляют каждую уникальную группу, которая просматривается в определении расписания.</span><span class="sxs-lookup"><span data-stu-id="da964-108">Instances also represent each unique group being reviewed in the schedule definition.</span></span> <span data-ttu-id="da964-109">Если в определении расписания просматриваются несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения.</span><span class="sxs-lookup"><span data-stu-id="da964-109">If a schedule definition reviews multiple groups, each group will have a unique instance for each recurrence.</span></span>

<span data-ttu-id="da964-110">Каждый **акцессревиевинстанце** содержит список [решений](accessreviewinstancedecisionitem.md) , на которые могут выполнять действия проверяющих.</span><span class="sxs-lookup"><span data-stu-id="da964-110">Every **accessReviewInstance** contains a list of [decisions](accessreviewinstancedecisionitem.md) that reviewers can take action on.</span></span> <span data-ttu-id="da964-111">Для рассмотрения одного и того же удостоверения существует одно решение.</span><span class="sxs-lookup"><span data-stu-id="da964-111">There is one decision per identity being reviewed.</span></span>

## <a name="methods"></a><span data-ttu-id="da964-112">Методы</span><span class="sxs-lookup"><span data-stu-id="da964-112">Methods</span></span>

| <span data-ttu-id="da964-113">Метод</span><span class="sxs-lookup"><span data-stu-id="da964-113">Method</span></span> | <span data-ttu-id="da964-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da964-114">Return Type</span></span> | <span data-ttu-id="da964-115">Описание</span><span class="sxs-lookup"><span data-stu-id="da964-115">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="da964-116">Список Акцессревиевинстанцес</span><span class="sxs-lookup"><span data-stu-id="da964-116">List accessReviewInstances</span></span>](../api/accessreviewinstance-list.md) | <span data-ttu-id="da964-117">Коллекция [акцессревиевинстанце](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="da964-117">[accessReviewInstance](accessreviewinstance.md) collection</span></span> | <span data-ttu-id="da964-118">Получение списка объектов [акцессревиевинстанце](../resources/accessreviewinstance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="da964-118">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span> |
|[<span data-ttu-id="da964-119">Получение Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="da964-119">Get accessReviewInstance</span></span>](../api/accessreviewinstance-get.md) | [<span data-ttu-id="da964-120">акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="da964-120">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="da964-121">Возвращает Акцессревиевинстанце для Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="da964-121">Returns accessReviewInstance for an accessReviewScheduleDefinition.</span></span> <span data-ttu-id="da964-122">Не включает в объект связанное АкцессревиевинстанцедеЦисионитем.</span><span class="sxs-lookup"><span data-stu-id="da964-122">Does not include associated accessReviewInstanceDecisionItem\`s in the object.</span></span> |
|[<span data-ttu-id="da964-123">Список Пендингакцессревиевинстанцес</span><span class="sxs-lookup"><span data-stu-id="da964-123">List pendingAccessReviewInstances</span></span>](../api/accessreviewinstance-pendingaccessreviewinstances.md) | <span data-ttu-id="da964-124">Коллекция [акцессревиевинстанце](accessreviewinstance.md) .</span><span class="sxs-lookup"><span data-stu-id="da964-124">[accessReviewInstance](accessreviewinstance.md) collection.</span></span> | <span data-ttu-id="da964-125">Получение всех ожидающих Акцессревиевинстанце ресурсов, назначенных вызывающему пользователю.</span><span class="sxs-lookup"><span data-stu-id="da964-125">Get all pending accessReviewInstance resources assigned to the calling user.</span></span> |
|[<span data-ttu-id="da964-126">Отправка напоминания о Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="da964-126">Send accessReviewInstance reminder</span></span>](../api/accessreviewinstance-sendreminder.md) | <span data-ttu-id="da964-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="da964-127">None.</span></span> | <span data-ttu-id="da964-128">Отправьте напоминание рецензентам Акцессревиевинстанце.</span><span class="sxs-lookup"><span data-stu-id="da964-128">Send a reminder to the reviewers of an accessReviewInstance.</span></span> |
|[<span data-ttu-id="da964-129">Остановить Акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="da964-129">Stop accessReviewInstance</span></span>](../api/accessreviewinstance-stop.md) | <span data-ttu-id="da964-130">Нет.</span><span class="sxs-lookup"><span data-stu-id="da964-130">None.</span></span> | <span data-ttu-id="da964-131">Вручную остановите Акцессревиевинстанце.</span><span class="sxs-lookup"><span data-stu-id="da964-131">Manually stop an accessReviewInstance.</span></span> |
|[<span data-ttu-id="da964-132">Принятие рекомендаций</span><span class="sxs-lookup"><span data-stu-id="da964-132">Accept recommendations</span></span>](../api/accessreviewinstance-acceptrecommendations.md) | <span data-ttu-id="da964-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="da964-133">None.</span></span> | <span data-ttu-id="da964-134">Позволяет вызывающему пользователю принимать рекомендации по решению для каждого Нотревиевед АкцессревиевинстанцедеЦисионитем, на которые они пересматриваются для определенного Акцессревиевинстанце.</span><span class="sxs-lookup"><span data-stu-id="da964-134">Allows the calling user to accept the decision recommendation for each NotReviewed accessReviewInstanceDecisionItem that they are the reviewer on for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="da964-135">Применение решений</span><span class="sxs-lookup"><span data-stu-id="da964-135">Apply decisions</span></span>](../api/accessreviewinstance-applydecisions.md) | <span data-ttu-id="da964-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="da964-136">None.</span></span> | <span data-ttu-id="da964-137">Вручную применяйте решение для Акцессревиевинстанце.</span><span class="sxs-lookup"><span data-stu-id="da964-137">Manually apply decision on an accessReviewInstance.</span></span> |



## <a name="properties"></a><span data-ttu-id="da964-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="da964-138">Properties</span></span>
| <span data-ttu-id="da964-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="da964-139">Property</span></span> | <span data-ttu-id="da964-140">Тип</span><span class="sxs-lookup"><span data-stu-id="da964-140">Type</span></span> | <span data-ttu-id="da964-141">Описание</span><span class="sxs-lookup"><span data-stu-id="da964-141">Description</span></span> |
| :-------------------------| :---------------------------------- | :---------- |
| <span data-ttu-id="da964-142">id</span><span class="sxs-lookup"><span data-stu-id="da964-142">id</span></span> | <span data-ttu-id="da964-143">Строка</span><span class="sxs-lookup"><span data-stu-id="da964-143">String</span></span> | <span data-ttu-id="da964-144">Уникальный идентификатор экземпляра.</span><span class="sxs-lookup"><span data-stu-id="da964-144">Unique identifier of the instance.</span></span> |
| <span data-ttu-id="da964-145">displayName</span><span class="sxs-lookup"><span data-stu-id="da964-145">displayName</span></span> | <span data-ttu-id="da964-146">Строка</span><span class="sxs-lookup"><span data-stu-id="da964-146">String</span></span> | <span data-ttu-id="da964-147">Имя родительского Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="da964-147">Name of the parent accessReviewScheduleDefinition.</span></span> |
| <span data-ttu-id="da964-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da964-148">startDateTime</span></span> | <span data-ttu-id="da964-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da964-149">DateTimeOffset</span></span> | <span data-ttu-id="da964-150">DateTime при запланированном запуске проверки экземпляра.</span><span class="sxs-lookup"><span data-stu-id="da964-150">DateTime when review instance is scheduled to start.</span></span> <span data-ttu-id="da964-151">Может быть в будущем.</span><span class="sxs-lookup"><span data-stu-id="da964-151">May be in the future.</span></span> |
| <span data-ttu-id="da964-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="da964-152">endDateTime</span></span> | <span data-ttu-id="da964-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da964-153">DateTimeOffset</span></span> | <span data-ttu-id="da964-154">DateTime при запланированном окончании проверки экземпляра.</span><span class="sxs-lookup"><span data-stu-id="da964-154">DateTime when review instance is scheduled to end.</span></span> |
| <span data-ttu-id="da964-155">status</span><span class="sxs-lookup"><span data-stu-id="da964-155">status</span></span> | <span data-ttu-id="da964-156">string</span><span class="sxs-lookup"><span data-stu-id="da964-156">string</span></span> | <span data-ttu-id="da964-157">Указывает состояние Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="da964-157">Specifies the status of an accessReview.</span></span> <span data-ttu-id="da964-158">Типичные состояния:,,,,, `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` , `AutoReviewing` и `AutoReviewed` .</span><span class="sxs-lookup"><span data-stu-id="da964-158">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span>  <span data-ttu-id="da964-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da964-159">Read-only.</span></span>|
| <span data-ttu-id="da964-160">scope</span><span class="sxs-lookup"><span data-stu-id="da964-160">scope</span></span> | [<span data-ttu-id="da964-161">акцессревиевскопе</span><span class="sxs-lookup"><span data-stu-id="da964-161">accessReviewScope</span></span>](accessreviewscope.md) | <span data-ttu-id="da964-162">Создается на основе **области действия** и **Инстанцеенумератионскопе** на уровне акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="da964-162">Created based on **scope** and **instanceEnumerationScope** at the accessReviewScheduleDefinition level.</span></span> <span data-ttu-id="da964-163">Определяет область пользователей, проверенных в группе.</span><span class="sxs-lookup"><span data-stu-id="da964-163">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="da964-164">В случае с проверкой одной группы область, определенная на `accessReviewScheduleDefinition` уровне, применяется ко всем экземплярам.</span><span class="sxs-lookup"><span data-stu-id="da964-164">In the case of a single-group review, the scope defined at the `accessReviewScheduleDefinition` level applies to all instances.</span></span> <span data-ttu-id="da964-165">В случае проверки всех групп область может различаться для каждой группы.</span><span class="sxs-lookup"><span data-stu-id="da964-165">In the case of all groups review, scope may be different for each group.</span></span> <span data-ttu-id="da964-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da964-166">Read-only.</span></span>  | 
| <span data-ttu-id="da964-167">решения</span><span class="sxs-lookup"><span data-stu-id="da964-167">decisions</span></span> | <span data-ttu-id="da964-168">Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="da964-168">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="da964-169">Каждый пользователь, который просматривается в Акцессревиевинстанце, имеет элемент принятия решений, который представляет, был ли их доступ утвержден, отклонен или еще не проверен.</span><span class="sxs-lookup"><span data-stu-id="da964-169">Each user reviewed in an accessReviewInstance has a decision item representing if their access was approved, denied, or not yet reviewed.</span></span> |
| <span data-ttu-id="da964-170">RDLC</span><span class="sxs-lookup"><span data-stu-id="da964-170">definition</span></span> |[<span data-ttu-id="da964-171">акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="da964-171">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="da964-172">С каждым экземпляром связан ровно один Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="da964-172">There is exactly one accessReviewScheduleDefinition associated with each instance.</span></span> <span data-ttu-id="da964-173">Это родительское расписание для экземпляра, в котором экземпляры создаются для каждого повторения определения проверки и каждая группа, выбранная для просмотра определением.</span><span class="sxs-lookup"><span data-stu-id="da964-173">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |

## <a name="relationships"></a><span data-ttu-id="da964-174">Связи</span><span class="sxs-lookup"><span data-stu-id="da964-174">Relationships</span></span>

| <span data-ttu-id="da964-175">Связь</span><span class="sxs-lookup"><span data-stu-id="da964-175">Relationship</span></span> | <span data-ttu-id="da964-176">Тип</span><span class="sxs-lookup"><span data-stu-id="da964-176">Type</span></span>   |<span data-ttu-id="da964-177">Описание</span><span class="sxs-lookup"><span data-stu-id="da964-177">Description</span></span>|
|:---------------|:--------|:----------|
| `definition`               |[<span data-ttu-id="da964-178">акцессревиевсчедуледефинитион</span><span class="sxs-lookup"><span data-stu-id="da964-178">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md)          | <span data-ttu-id="da964-179">`accessReviewScheduleDefinition`С каждым экземпляром связан только один экземпляр.</span><span class="sxs-lookup"><span data-stu-id="da964-179">There is exactly one `accessReviewScheduleDefinition` associated with each instance.</span></span> <span data-ttu-id="da964-180">Это родительское расписание для экземпляра, в котором экземпляры создаются для каждого повторения определения проверки и каждая группа, выбранная для просмотра определением.</span><span class="sxs-lookup"><span data-stu-id="da964-180">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |
| `decisions`               |<span data-ttu-id="da964-181">Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="da964-181">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span>        | <span data-ttu-id="da964-182">Каждый пользователь, проверенный в элементе, `accessReviewInstance` имеет элемент принятия решений, который представляет, было ли оно утверждено, отклонено или еще не проверено.</span><span class="sxs-lookup"><span data-stu-id="da964-182">Each user reviewed in an `accessReviewInstance` has a decision item representing if they were approved, denied, or not yet reviewed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da964-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da964-183">JSON representation</span></span>

<span data-ttu-id="da964-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da964-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
