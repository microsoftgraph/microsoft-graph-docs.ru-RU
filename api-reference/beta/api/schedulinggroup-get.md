---
title: Получение объекта schedulingGroup
description: Получение свойств и связей объекта [счедулингграуп](../resources/schedulinggroup.md) по идентификатору.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b8784aa4e3f5b2c77b0da185e5c3e5eb30856fa3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975741"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="af8be-103">Получение объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="af8be-103">Get schedulingGroup</span></span>

<span data-ttu-id="af8be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af8be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af8be-105">Получение свойств и связей объекта [счедулингграуп](../resources/schedulinggroup.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="af8be-105">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="af8be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af8be-106">Permissions</span></span>

<span data-ttu-id="af8be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af8be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af8be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af8be-109">Permission type</span></span>      | <span data-ttu-id="af8be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af8be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af8be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af8be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af8be-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af8be-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="af8be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af8be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af8be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af8be-114">Not supported.</span></span>    |
|<span data-ttu-id="af8be-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="af8be-115">Application</span></span> | <span data-ttu-id="af8be-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="af8be-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af8be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af8be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af8be-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="af8be-118">Optional query parameters</span></span>

<span data-ttu-id="af8be-119">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="af8be-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af8be-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af8be-120">Request headers</span></span>

| <span data-ttu-id="af8be-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af8be-121">Header</span></span>       | <span data-ttu-id="af8be-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af8be-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="af8be-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af8be-123">Authorization</span></span>  | <span data-ttu-id="af8be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af8be-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af8be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af8be-126">Request body</span></span>
<span data-ttu-id="af8be-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af8be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af8be-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="af8be-128">Response</span></span>

<span data-ttu-id="af8be-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af8be-129">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af8be-130">Пример</span><span class="sxs-lookup"><span data-stu-id="af8be-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="af8be-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="af8be-131">Request</span></span>

<span data-ttu-id="af8be-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af8be-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af8be-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="af8be-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="af8be-134">C#</span><span class="sxs-lookup"><span data-stu-id="af8be-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af8be-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af8be-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af8be-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af8be-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af8be-137">Java</span><span class="sxs-lookup"><span data-stu-id="af8be-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-get-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="af8be-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="af8be-138">Response</span></span>

<span data-ttu-id="af8be-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af8be-139">The following is an example of the response.</span></span> 

><span data-ttu-id="af8be-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af8be-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a schedulingGroup by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


