---
title: Получение смены
description: Получение сдвига по ИДЕНТИФИКАТОРу.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dbeedc59e39e6efe06a2989199ef53d7ced20b1e
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216688"
---
# <a name="get-shift"></a><span data-ttu-id="4e812-103">Получение смены</span><span class="sxs-lookup"><span data-stu-id="4e812-103">Get shift</span></span>

<span data-ttu-id="4e812-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e812-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e812-105">Получение свойств и связей объекта [SHIFT](../resources/shift.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="4e812-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e812-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e812-106">Permissions</span></span>

<span data-ttu-id="4e812-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e812-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e812-109">Permission type</span></span>      | <span data-ttu-id="4e812-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e812-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e812-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e812-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4e812-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e812-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e812-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e812-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e812-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e812-114">Not supported.</span></span>    |<span data-ttu-id="4e812-115">s</span><span class="sxs-lookup"><span data-stu-id="4e812-115">s</span></span>
|<span data-ttu-id="4e812-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e812-116">Application</span></span> | <span data-ttu-id="4e812-117">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4e812-117">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="4e812-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="4e812-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4e812-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="4e812-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4e812-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e812-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e812-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e812-121">Optional query parameters</span></span>

<span data-ttu-id="4e812-122">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4e812-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e812-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e812-123">Request headers</span></span>

| <span data-ttu-id="4e812-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e812-124">Header</span></span>       | <span data-ttu-id="4e812-125">Значение</span><span class="sxs-lookup"><span data-stu-id="4e812-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e812-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e812-126">Authorization</span></span>  | <span data-ttu-id="4e812-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e812-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e812-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e812-129">Request body</span></span>
<span data-ttu-id="4e812-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e812-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e812-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e812-131">Response</span></span>

<span data-ttu-id="4e812-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e812-132">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e812-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4e812-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e812-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e812-134">Request</span></span>

<span data-ttu-id="4e812-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e812-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e812-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e812-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="4e812-137">C#</span><span class="sxs-lookup"><span data-stu-id="4e812-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e812-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e812-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e812-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e812-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e812-140">Java</span><span class="sxs-lookup"><span data-stu-id="4e812-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="4e812-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e812-141">Response</span></span>

<span data-ttu-id="4e812-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e812-142">The following is an example of the response.</span></span>

><span data-ttu-id="4e812-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e812-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
