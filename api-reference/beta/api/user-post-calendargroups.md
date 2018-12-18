---
title: Создание объекта CalendarGroup
description: С помощью этого API можно создать экземпляр CalendarGroup.
author: dkershaw10
ms.openlocfilehash: a68be3470489b20667112b67d15f4472a3817d4b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319050"
---
# <a name="create-calendargroup"></a><span data-ttu-id="8d580-103">Создание объекта CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="8d580-103">Create CalendarGroup</span></span>

> <span data-ttu-id="8d580-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d580-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d580-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d580-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d580-106">С помощью этого API можно создать экземпляр CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="8d580-106">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d580-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d580-107">Permissions</span></span>
<span data-ttu-id="8d580-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d580-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d580-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d580-110">Permission type</span></span>      | <span data-ttu-id="8d580-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d580-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d580-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d580-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d580-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d580-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8d580-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d580-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d580-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d580-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8d580-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d580-116">Application</span></span> | <span data-ttu-id="8d580-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d580-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d580-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d580-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="8d580-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d580-119">Request headers</span></span>
| <span data-ttu-id="8d580-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d580-120">Header</span></span>       | <span data-ttu-id="8d580-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d580-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d580-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d580-122">Authorization</span></span>  | <span data-ttu-id="8d580-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d580-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8d580-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d580-125">Content-Type</span></span>  | <span data-ttu-id="8d580-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d580-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d580-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d580-127">Request body</span></span>
<span data-ttu-id="8d580-128">Предоставьте в тексте запроса описание объекта [CalendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d580-128">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8d580-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d580-129">Response</span></span>

<span data-ttu-id="8d580-130">В случае успеха этот метод возвращает код отклика `201 Created` и объект [CalendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d580-130">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d580-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8d580-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d580-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d580-132">Request</span></span>
<span data-ttu-id="8d580-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d580-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="8d580-134">Предоставьте в тексте запроса описание объекта [calendarGroup](../resources/calendargroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d580-134">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8d580-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d580-135">Response</span></span>
<span data-ttu-id="8d580-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8d580-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
