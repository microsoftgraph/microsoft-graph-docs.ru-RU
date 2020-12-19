---
title: Создание объекта Calendar
description: С помощью этого API можно для экземпляра user создать календарь в группе календарей.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 76154531f45bca34772ece6145a34d67063a5c86
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719582"
---
# <a name="create-calendar"></a><span data-ttu-id="bcabe-103">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="bcabe-103">Create Calendar</span></span>

<span data-ttu-id="bcabe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcabe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bcabe-105">С помощью этого API можно для экземпляра [user](../resources/user.md) создать календарь в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="bcabe-105">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bcabe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcabe-106">Permissions</span></span>

<span data-ttu-id="bcabe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcabe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bcabe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcabe-109">Permission type</span></span>                        | <span data-ttu-id="bcabe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcabe-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bcabe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcabe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bcabe-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcabe-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="bcabe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcabe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcabe-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcabe-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="bcabe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcabe-115">Application</span></span>                            | <span data-ttu-id="bcabe-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bcabe-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bcabe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcabe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="bcabe-118">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcabe-118">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="bcabe-119">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcabe-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="bcabe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcabe-120">Request headers</span></span>

| <span data-ttu-id="bcabe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcabe-121">Header</span></span>        | <span data-ttu-id="bcabe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bcabe-122">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="bcabe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcabe-123">Authorization</span></span> | <span data-ttu-id="bcabe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcabe-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bcabe-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcabe-126">Content-Type</span></span>  | <span data-ttu-id="bcabe-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcabe-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcabe-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcabe-129">Request body</span></span>

<span data-ttu-id="bcabe-130">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcabe-130">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bcabe-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcabe-131">Response</span></span>

<span data-ttu-id="bcabe-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcabe-132">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcabe-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bcabe-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bcabe-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcabe-134">Request</span></span>

<span data-ttu-id="bcabe-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcabe-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bcabe-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcabe-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAR9NR5AAA="],
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars
Content-type: application/json

{
  "name": "Marketing calendar"
}
```
# <a name="javascript"></a>[<span data-ttu-id="bcabe-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcabe-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="bcabe-138">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcabe-138">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="bcabe-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcabe-139">Response</span></span>

<span data-ttu-id="bcabe-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcabe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/calendarGroups('AAMkADYAAAR9NR5AAA%3D')/calendars/$entity",
    "id": "AAMkADYCQM0GfRAAAcrRD-AAA=",
    "name": "Marketing calendar",
    "color": "auto",
    "changeKey": "4xTfgHLeDkOqYVAkDNBn0QAAHKl46A==",
    "canShare": true,
    "canViewPrivateItems": true,
    "canEdit": true,
    "owner": {
        "name": "Adele Vance",
        "address": "adelev@contoso.OnMicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

