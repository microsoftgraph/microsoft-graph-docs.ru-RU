---
title: Получение объекта calendarGroup
description: Получение свойств и связей, принадлежащих объекту группы календарей.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7288e5e96c4a32464d6e8a2574cd356f26d5c462
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047716"
---
# <a name="get-calendargroup"></a><span data-ttu-id="aac86-103">Получение объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="aac86-103">Get calendarGroup</span></span>

<span data-ttu-id="aac86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aac86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aac86-105">Получение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="aac86-105">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aac86-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aac86-106">Permissions</span></span>

<span data-ttu-id="aac86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aac86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aac86-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aac86-109">Permission type</span></span>                        | <span data-ttu-id="aac86-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aac86-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="aac86-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aac86-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aac86-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aac86-112">Calendars.Read</span></span>                              |
| <span data-ttu-id="aac86-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aac86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aac86-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aac86-114">Calendars.Read</span></span>                              |
| <span data-ttu-id="aac86-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aac86-115">Application</span></span>                            | <span data-ttu-id="aac86-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aac86-116">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="aac86-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aac86-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="aac86-118">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="aac86-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aac86-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aac86-119">Optional query parameters</span></span>

<span data-ttu-id="aac86-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aac86-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aac86-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aac86-121">Request headers</span></span>

| <span data-ttu-id="aac86-122">Имя</span><span class="sxs-lookup"><span data-stu-id="aac86-122">Name</span></span>          | <span data-ttu-id="aac86-123">Тип</span><span class="sxs-lookup"><span data-stu-id="aac86-123">Type</span></span>   | <span data-ttu-id="aac86-124">Описание</span><span class="sxs-lookup"><span data-stu-id="aac86-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="aac86-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac86-125">Authorization</span></span> | <span data-ttu-id="aac86-126">string</span><span class="sxs-lookup"><span data-stu-id="aac86-126">string</span></span> | <span data-ttu-id="aac86-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aac86-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aac86-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aac86-129">Request body</span></span>

<span data-ttu-id="aac86-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aac86-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aac86-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="aac86-131">Response</span></span>

<span data-ttu-id="aac86-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aac86-132">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac86-133">Пример</span><span class="sxs-lookup"><span data-stu-id="aac86-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aac86-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="aac86-134">Request</span></span>

<span data-ttu-id="aac86-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aac86-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="aac86-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="aac86-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="aac86-137">C#</span><span class="sxs-lookup"><span data-stu-id="aac86-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aac86-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aac86-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aac86-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aac86-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aac86-140">Java</span><span class="sxs-lookup"><span data-stu-id="aac86-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aac86-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="aac86-141">Response</span></span>

<span data-ttu-id="aac86-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aac86-142">Here is an example of the response.</span></span> <span data-ttu-id="aac86-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="aac86-143">Note: The response object shown here might be shortened for readability.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
