---
title: 'Расписание: общий доступ'
description: Предоставьте общий доступ к диапазону расписания с участниками расписания.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5a650b4ac6cab35dcbb9d4dce488201418752f55
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866961"
---
# <a name="schedule-share"></a><span data-ttu-id="06cb1-103">Расписание: общий доступ</span><span class="sxs-lookup"><span data-stu-id="06cb1-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06cb1-104">Предоставьте общий доступ к диапазону [расписания](../resources/schedule.md) с участниками расписания.</span><span class="sxs-lookup"><span data-stu-id="06cb1-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="06cb1-105">Сделайте коллекции элементов [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в указанном диапазоне времени [расписания](../resources/schedule.md) , отображаемого указанными участниками группы, включая "сотрудники" и "руководители".</span><span class="sxs-lookup"><span data-stu-id="06cb1-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="06cb1-106">Каждый экземпляр [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в [расписании](../resources/schedule.md) поддерживает черновую и общую версии элемента.</span><span class="sxs-lookup"><span data-stu-id="06cb1-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="06cb1-107">Черновая версия доступна для просмотра только руководителями, а общая версия доступна для просмотра сотрудниками и руководителями.</span><span class="sxs-lookup"><span data-stu-id="06cb1-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="06cb1-108">Для каждого экземпляра [SHIFT](../resources/shift.md) и [тимеофф](../resources/timeoff.md) в указанном диапазоне времени, действие Share обновляет общую версию из черновой версии, поэтому в дополнение к менеджерам сотрудники также могут просматривать самую актуальную информацию об элементе.</span><span class="sxs-lookup"><span data-stu-id="06cb1-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="06cb1-109">Параметр **нотифитеам** указывает, какие сотрудники могут просматривать элемент.</span><span class="sxs-lookup"><span data-stu-id="06cb1-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="06cb1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06cb1-110">Permissions</span></span>

<span data-ttu-id="06cb1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06cb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06cb1-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06cb1-113">Permission type</span></span>      | <span data-ttu-id="06cb1-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06cb1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06cb1-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06cb1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="06cb1-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06cb1-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="06cb1-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06cb1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06cb1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06cb1-118">Not supported.</span></span>    |
|<span data-ttu-id="06cb1-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="06cb1-119">Application</span></span> | <span data-ttu-id="06cb1-120">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="06cb1-120">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="06cb1-121">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="06cb1-121">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="06cb1-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="06cb1-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="06cb1-123">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="06cb1-123">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="06cb1-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06cb1-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="06cb1-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06cb1-125">Request headers</span></span>

| <span data-ttu-id="06cb1-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06cb1-126">Header</span></span>       | <span data-ttu-id="06cb1-127">Значение</span><span class="sxs-lookup"><span data-stu-id="06cb1-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06cb1-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06cb1-128">Authorization</span></span>  | <span data-ttu-id="06cb1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06cb1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="06cb1-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06cb1-131">Content-Type</span></span>  | <span data-ttu-id="06cb1-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06cb1-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06cb1-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06cb1-134">Request body</span></span>

<span data-ttu-id="06cb1-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="06cb1-135">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="06cb1-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="06cb1-136">Parameter</span></span>                   |<span data-ttu-id="06cb1-137">Тип</span><span class="sxs-lookup"><span data-stu-id="06cb1-137">Type</span></span>           |<span data-ttu-id="06cb1-138">Описание</span><span class="sxs-lookup"><span data-stu-id="06cb1-138">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="06cb1-139">нотифитеам</span><span class="sxs-lookup"><span data-stu-id="06cb1-139">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="06cb1-140">Указывает, должна ли вся группа получить видимое уведомление о данном действии или только те сотрудники, которым назначена смена.</span><span class="sxs-lookup"><span data-stu-id="06cb1-140">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="06cb1-141">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="06cb1-141">Required.</span></span>       |
| <span data-ttu-id="06cb1-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06cb1-142">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="06cb1-143">Время начала совместного использования смен по расписанию.</span><span class="sxs-lookup"><span data-stu-id="06cb1-143">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="06cb1-144">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="06cb1-144">Required.</span></span>   |
| <span data-ttu-id="06cb1-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="06cb1-145">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="06cb1-146">Время окончания для совместного использования смены графика до.</span><span class="sxs-lookup"><span data-stu-id="06cb1-146">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="06cb1-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="06cb1-147">Response</span></span>

<span data-ttu-id="06cb1-p108">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="06cb1-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06cb1-150">Пример</span><span class="sxs-lookup"><span data-stu-id="06cb1-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="06cb1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="06cb1-151">Request</span></span>

<span data-ttu-id="06cb1-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06cb1-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="06cb1-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="06cb1-153">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="06cb1-154">C#</span><span class="sxs-lookup"><span data-stu-id="06cb1-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06cb1-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06cb1-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06cb1-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06cb1-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="06cb1-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="06cb1-157">Response</span></span>

<span data-ttu-id="06cb1-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="06cb1-158">The following is an example of the response.</span></span> 

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
