---
title: Создание объекта Calendar
description: С помощью этого API можно создать календарь для экземпляра user.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 867641a47ca02e903c22a3338a0fe87f7c70bddf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887824"
---
# <a name="create-calendar"></a><span data-ttu-id="13b94-103">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="13b94-103">Create Calendar</span></span>

> <span data-ttu-id="13b94-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13b94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13b94-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13b94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13b94-106">С помощью этого API можно создать календарь для экземпляра [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="13b94-106">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="13b94-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13b94-107">Permissions</span></span>
<span data-ttu-id="13b94-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13b94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13b94-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13b94-110">Permission type</span></span>      | <span data-ttu-id="13b94-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13b94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13b94-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13b94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="13b94-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13b94-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="13b94-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13b94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13b94-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13b94-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="13b94-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13b94-116">Application</span></span> | <span data-ttu-id="13b94-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13b94-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="13b94-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13b94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="13b94-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13b94-119">Request headers</span></span>
| <span data-ttu-id="13b94-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13b94-120">Header</span></span>       | <span data-ttu-id="13b94-121">Значение</span><span class="sxs-lookup"><span data-stu-id="13b94-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13b94-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13b94-122">Authorization</span></span>  | <span data-ttu-id="13b94-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13b94-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="13b94-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="13b94-125">Content-Type</span></span>  | <span data-ttu-id="13b94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13b94-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13b94-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13b94-127">Request body</span></span>
<span data-ttu-id="13b94-128">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13b94-128">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="13b94-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="13b94-129">Response</span></span>

<span data-ttu-id="13b94-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13b94-130">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13b94-131">Пример</span><span class="sxs-lookup"><span data-stu-id="13b94-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13b94-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="13b94-132">Request</span></span>
<span data-ttu-id="13b94-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13b94-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}

```
<span data-ttu-id="13b94-134">Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13b94-134">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="13b94-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="13b94-135">Response</span></span>
<span data-ttu-id="13b94-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="13b94-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
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
  "tocPath": ""
}-->
