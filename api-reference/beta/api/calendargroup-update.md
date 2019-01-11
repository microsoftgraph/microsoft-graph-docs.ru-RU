---
title: Обновление объекта calendarGroup.
description: Обновление свойств объекта calendargroup.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9a8006098c1088caec444b30aa5210b44388f5cf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809403"
---
# <a name="update-calendargroup"></a><span data-ttu-id="46b8a-103">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="46b8a-103">Update calendargroup</span></span>

> <span data-ttu-id="46b8a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46b8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46b8a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46b8a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46b8a-106">Обновление свойств объекта calendargroup.</span><span class="sxs-lookup"><span data-stu-id="46b8a-106">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46b8a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46b8a-107">Permissions</span></span>

<span data-ttu-id="46b8a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46b8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46b8a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46b8a-110">Permission type</span></span>                        | <span data-ttu-id="46b8a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46b8a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="46b8a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46b8a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="46b8a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46b8a-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="46b8a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46b8a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46b8a-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46b8a-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="46b8a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46b8a-116">Application</span></span>                            | <span data-ttu-id="46b8a-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46b8a-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="46b8a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46b8a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="46b8a-119">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="46b8a-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="46b8a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46b8a-120">Request headers</span></span>

| <span data-ttu-id="46b8a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46b8a-121">Header</span></span>        | <span data-ttu-id="46b8a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46b8a-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="46b8a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46b8a-123">Authorization</span></span> | <span data-ttu-id="46b8a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46b8a-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="46b8a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46b8a-126">Content-Type</span></span>  | <span data-ttu-id="46b8a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46b8a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46b8a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46b8a-129">Request body</span></span>

<span data-ttu-id="46b8a-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="46b8a-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="46b8a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="46b8a-133">Property</span></span> | <span data-ttu-id="46b8a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="46b8a-134">Type</span></span>   | <span data-ttu-id="46b8a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="46b8a-135">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="46b8a-136">name</span><span class="sxs-lookup"><span data-stu-id="46b8a-136">name</span></span>     | <span data-ttu-id="46b8a-137">String</span><span class="sxs-lookup"><span data-stu-id="46b8a-137">String</span></span> | <span data-ttu-id="46b8a-138">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="46b8a-138">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="46b8a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="46b8a-139">Response</span></span>

<span data-ttu-id="46b8a-140">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46b8a-140">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b8a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="46b8a-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="46b8a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="46b8a-142">Request</span></span>

<span data-ttu-id="46b8a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46b8a-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="46b8a-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="46b8a-144">Response</span></span>

<span data-ttu-id="46b8a-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46b8a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
