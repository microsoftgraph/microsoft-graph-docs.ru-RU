---
title: Получение объекта calendarGroup
description: Получение свойств и связей, принадлежащих объекту группы календарей.
ms.openlocfilehash: ffaf4fa4fbc96649bb93a430e77be758e8768ceb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026910"
---
# <a name="get-calendargroup"></a><span data-ttu-id="a6313-103">Получение объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a6313-103">Get calendarGroup</span></span>

<span data-ttu-id="a6313-104">Получение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="a6313-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6313-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6313-105">Permissions</span></span>

<span data-ttu-id="a6313-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6313-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6313-108">Permission type</span></span>                        | <span data-ttu-id="a6313-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6313-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a6313-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6313-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6313-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a6313-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="a6313-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6313-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6313-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a6313-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="a6313-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6313-114">Application</span></span>                            | <span data-ttu-id="a6313-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a6313-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="a6313-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6313-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="a6313-117">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="a6313-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6313-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6313-118">Optional query parameters</span></span>

<span data-ttu-id="a6313-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6313-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6313-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6313-120">Request headers</span></span>

| <span data-ttu-id="a6313-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a6313-121">Name</span></span>          | <span data-ttu-id="a6313-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a6313-122">Type</span></span>   | <span data-ttu-id="a6313-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a6313-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="a6313-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6313-124">Authorization</span></span> | <span data-ttu-id="a6313-125">string</span><span class="sxs-lookup"><span data-stu-id="a6313-125">string</span></span> | <span data-ttu-id="a6313-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6313-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6313-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6313-128">Request body</span></span>

<span data-ttu-id="a6313-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6313-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6313-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6313-130">Response</span></span>

<span data-ttu-id="a6313-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6313-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6313-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a6313-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6313-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6313-133">Request</span></span>

<span data-ttu-id="a6313-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6313-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="a6313-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6313-135">Response</span></span>

<span data-ttu-id="a6313-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a6313-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
