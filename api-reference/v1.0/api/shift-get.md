---
title: Получение смены
description: Получите смену по ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e4754e86ecaae0c39c519362c25ba08a49a5cbfb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054415"
---
# <a name="get-shift"></a><span data-ttu-id="ffd17-103">Получение смены</span><span class="sxs-lookup"><span data-stu-id="ffd17-103">Get shift</span></span>

<span data-ttu-id="ffd17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffd17-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffd17-105">Извлечение свойств и связей объекта [переноса](../resources/shift.md) по ID.</span><span class="sxs-lookup"><span data-stu-id="ffd17-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffd17-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd17-106">Permissions</span></span>

<span data-ttu-id="ffd17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffd17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="ffd17-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd17-109">Permission type</span></span>                        | <span data-ttu-id="ffd17-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffd17-110">Permissions (from least to most privileged)</span></span>                                    |
|:---------------------------------------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="ffd17-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffd17-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffd17-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffd17-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ffd17-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffd17-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffd17-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffd17-114">Not supported.</span></span>                                                                 |
| <span data-ttu-id="ffd17-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ffd17-115">Application</span></span>                            | <span data-ttu-id="ffd17-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffd17-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span>                                      |

## <a name="http-request"></a><span data-ttu-id="ffd17-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffd17-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffd17-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ffd17-118">Optional query parameters</span></span>

<span data-ttu-id="ffd17-119">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ffd17-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffd17-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffd17-120">Request headers</span></span>

| <span data-ttu-id="ffd17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffd17-121">Header</span></span>       | <span data-ttu-id="ffd17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ffd17-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ffd17-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffd17-123">Authorization</span></span>  | <span data-ttu-id="ffd17-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffd17-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ffd17-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffd17-126">Request body</span></span>
<span data-ttu-id="ffd17-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffd17-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffd17-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffd17-128">Response</span></span>

<span data-ttu-id="ffd17-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [переноса](../resources/shift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ffd17-129">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffd17-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ffd17-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffd17-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffd17-131">Request</span></span>

<span data-ttu-id="ffd17-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffd17-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ffd17-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffd17-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="ffd17-134">C#</span><span class="sxs-lookup"><span data-stu-id="ffd17-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffd17-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffd17-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffd17-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffd17-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffd17-137">Java</span><span class="sxs-lookup"><span data-stu-id="ffd17-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="ffd17-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffd17-138">Response</span></span>

<span data-ttu-id="ffd17-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ffd17-139">The following is an example of the response.</span></span>

><span data-ttu-id="ffd17-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ffd17-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHFT_ca485cdd-a42c-4b93-9e6a-6fa54fd45fe1",
    "createdDateTime": "2019-06-06T20:15:38.9Z",
    "lastModifiedDateTime": "2019-11-18T01:12:08.318Z",
    "schedulingGroupId": "TAG_d18fd675-3ac8-41b2-8038-d17fdac8b0d3",
    "userId": "a7b0c8c4-3f5c-492f-ab13-40f0e0f0ffa8",
    "draftShift": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "1c717a55-febd-4850-b5f6-101f3a29972c",
            "displayName": "Sumanth Lingom"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

