---
title: 'Расписание: общий доступ'
description: Предоставьте общий доступ к диапазону расписания с участниками расписания.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c25b0255afd4ca50a36e757eb16fb42f5c1c3a94
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982977"
---
# <a name="schedule-share"></a><span data-ttu-id="dfa5e-103">Расписание: общий доступ</span><span class="sxs-lookup"><span data-stu-id="dfa5e-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfa5e-104">Предоставьте общий доступ к диапазону [расписания](../resources/schedule.md) с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="dfa5e-105">Сделайте коллекции элементов [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в указанном диапазоне времени [расписания](../resources/schedule.md) , отображаемого указанными участниками группы, включая "сотрудники" и "руководители".</span><span class="sxs-lookup"><span data-stu-id="dfa5e-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="dfa5e-106">Каждый экземпляр [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в [расписании](../resources/schedule.md) поддерживает черновую и общую версии элемента.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="dfa5e-107">Черновая версия доступна для просмотра только руководителями, а общая версия доступна для просмотра сотрудниками и руководителями.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="dfa5e-108">Для каждого экземпляра [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в указанном диапазоне времени, действие Share обновляет общую версию из черновой версии, поэтому в дополнение к менеджерам сотрудники также могут просматривать самую актуальную информацию об элементе.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="dfa5e-109">Параметр **нотифитеам** указывает, какие сотрудники могут просматривать элемент.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfa5e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa5e-110">Permissions</span></span>

<span data-ttu-id="dfa5e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfa5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfa5e-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa5e-113">Permission type</span></span>      | <span data-ttu-id="dfa5e-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfa5e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfa5e-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfa5e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="dfa5e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa5e-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dfa5e-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfa5e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfa5e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-118">Not supported.</span></span>    |
|<span data-ttu-id="dfa5e-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfa5e-119">Application</span></span> | <span data-ttu-id="dfa5e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-120">Not supported.</span></span> |

> <span data-ttu-id="dfa5e-121">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="dfa5e-122">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="dfa5e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfa5e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="dfa5e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfa5e-124">Request headers</span></span>

| <span data-ttu-id="dfa5e-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfa5e-125">Header</span></span>       | <span data-ttu-id="dfa5e-126">Значение</span><span class="sxs-lookup"><span data-stu-id="dfa5e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dfa5e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfa5e-127">Authorization</span></span>  | <span data-ttu-id="dfa5e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dfa5e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfa5e-130">Content-Type</span></span>  | <span data-ttu-id="dfa5e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="dfa5e-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfa5e-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfa5e-132">Request body</span></span>

<span data-ttu-id="dfa5e-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="dfa5e-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="dfa5e-134">Parameter</span></span>                   |<span data-ttu-id="dfa5e-135">Тип</span><span class="sxs-lookup"><span data-stu-id="dfa5e-135">Type</span></span>           |<span data-ttu-id="dfa5e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa5e-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="dfa5e-137">Нотифитеам</span><span class="sxs-lookup"><span data-stu-id="dfa5e-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="dfa5e-138">Указывает, должна ли вся группа получить видимое уведомление о данном действии или только те сотрудники, которым назначена смена.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="dfa5e-139">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-139">Required.</span></span>       |
| <span data-ttu-id="dfa5e-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dfa5e-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="dfa5e-141">Время начала совместного использования смен по расписанию.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="dfa5e-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-142">Required.</span></span>   |
| <span data-ttu-id="dfa5e-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="dfa5e-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="dfa5e-144">Время окончания для совместного использования смены графика до.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="dfa5e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa5e-145">Response</span></span>

<span data-ttu-id="dfa5e-p107">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfa5e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="dfa5e-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dfa5e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa5e-149">Request</span></span>

<span data-ttu-id="dfa5e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-150">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dfa5e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfa5e-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dfa5e-152">C#</span><span class="sxs-lookup"><span data-stu-id="dfa5e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfa5e-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfa5e-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dfa5e-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dfa5e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dfa5e-155">Java</span><span class="sxs-lookup"><span data-stu-id="dfa5e-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-share-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dfa5e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa5e-156">Response</span></span>

<span data-ttu-id="dfa5e-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dfa5e-157">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
