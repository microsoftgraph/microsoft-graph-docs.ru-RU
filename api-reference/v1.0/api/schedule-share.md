---
title: 'Расписание: общий доступ'
description: Предоставьте общий доступ к диапазону расписания с участниками расписания.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 054a6dd0589929c22c7dc6b8c5e954dee360bef2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015661"
---
# <a name="schedule-share"></a><span data-ttu-id="a5af8-103">Расписание: общий доступ</span><span class="sxs-lookup"><span data-stu-id="a5af8-103">schedule: share</span></span>

<span data-ttu-id="a5af8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5af8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5af8-105">Предоставьте общий доступ к диапазону [расписания](../resources/schedule.md) с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="a5af8-105">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="a5af8-106">Сделайте коллекции элементов [SHIFT](../resources/shift.md), [опеншифт](../resources/openshift.md) и [тимеофф](../resources/timeoff.md) в указанном диапазоне времени [расписания](../resources/schedule.md) , отображаемых указанными участниками группы, включая "сотрудники" и "руководители".</span><span class="sxs-lookup"><span data-stu-id="a5af8-106">Make the collections of [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="a5af8-107">Каждый [из](../resources/shift.md)экземпляров [опеншифт](../resources/openshift.md) и [тимеофф](../resources/timeoff.md) в [расписании](../resources/schedule.md) поддерживает черновую и общую версии элемента.</span><span class="sxs-lookup"><span data-stu-id="a5af8-107">Each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="a5af8-108">Черновая версия доступна для просмотра только руководителями, а общая версия доступна для просмотра сотрудниками и руководителями.</span><span class="sxs-lookup"><span data-stu-id="a5af8-108">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="a5af8-109">Для каждого экземпляра [SHIFT](../resources/shift.md), [опеншифт](../resources/openshift.md) и [тимеофф](../resources/timeoff.md) в указанном диапазоне времени, действие Share обновляет общую версию из черновой версии, поэтому в дополнение к менеджерам сотрудники также могут просматривать самую актуальную информацию об элементе.</span><span class="sxs-lookup"><span data-stu-id="a5af8-109">For each [shift](../resources/shift.md), [openshift](../resources/openshift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="a5af8-110">Параметр **нотифитеам** указывает, какие сотрудники могут просматривать элемент.</span><span class="sxs-lookup"><span data-stu-id="a5af8-110">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5af8-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5af8-111">Permissions</span></span>

<span data-ttu-id="a5af8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5af8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5af8-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5af8-114">Permission type</span></span>      | <span data-ttu-id="a5af8-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5af8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5af8-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5af8-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a5af8-117">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a5af8-117">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5af8-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5af8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5af8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5af8-119">Not supported.</span></span>    |
|<span data-ttu-id="a5af8-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5af8-120">Application</span></span> | <span data-ttu-id="a5af8-121">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5af8-121">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="a5af8-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a5af8-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a5af8-123">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="a5af8-123">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a5af8-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5af8-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="a5af8-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5af8-125">Request headers</span></span>

| <span data-ttu-id="a5af8-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5af8-126">Header</span></span>       | <span data-ttu-id="a5af8-127">Значение</span><span class="sxs-lookup"><span data-stu-id="a5af8-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5af8-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5af8-128">Authorization</span></span>  | <span data-ttu-id="a5af8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5af8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5af8-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5af8-131">Content-Type</span></span>  | <span data-ttu-id="a5af8-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5af8-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5af8-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5af8-134">Request body</span></span>

<span data-ttu-id="a5af8-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a5af8-135">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="a5af8-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="a5af8-136">Parameter</span></span>                   |<span data-ttu-id="a5af8-137">Тип</span><span class="sxs-lookup"><span data-stu-id="a5af8-137">Type</span></span>           |<span data-ttu-id="a5af8-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a5af8-138">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="a5af8-139">нотифитеам</span><span class="sxs-lookup"><span data-stu-id="a5af8-139">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="a5af8-140">Указывает, должна ли вся группа получить видимое уведомление о данном действии или только те сотрудники, которым назначена смена.</span><span class="sxs-lookup"><span data-stu-id="a5af8-140">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="a5af8-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a5af8-141">Required.</span></span>       |
| <span data-ttu-id="a5af8-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a5af8-142">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="a5af8-143">Время начала совместного использования смен по расписанию.</span><span class="sxs-lookup"><span data-stu-id="a5af8-143">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="a5af8-144">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="a5af8-144">Required.</span></span>   |
| <span data-ttu-id="a5af8-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a5af8-145">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="a5af8-146">Время окончания для совместного использования смены графика до.</span><span class="sxs-lookup"><span data-stu-id="a5af8-146">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="a5af8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5af8-147">Response</span></span>

<span data-ttu-id="a5af8-p108">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5af8-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5af8-150">Пример</span><span class="sxs-lookup"><span data-stu-id="a5af8-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5af8-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5af8-151">Request</span></span>

<span data-ttu-id="a5af8-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5af8-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a5af8-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5af8-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```
# <a name="c"></a>[<span data-ttu-id="a5af8-154">C#</span><span class="sxs-lookup"><span data-stu-id="a5af8-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5af8-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5af8-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5af8-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5af8-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5af8-157">Java</span><span class="sxs-lookup"><span data-stu-id="a5af8-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-share-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="a5af8-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5af8-158">Response</span></span>

<span data-ttu-id="a5af8-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5af8-159">The following is an example of the response.</span></span> 

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

