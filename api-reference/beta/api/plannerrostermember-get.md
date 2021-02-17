---
title: Get plannerRosterMember
description: Чтение свойств и связей объекта plannerRosterMember.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 69ccf29dda22790f33f77458e0537667653b329f
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272356"
---
# <a name="get-plannerrostermember"></a><span data-ttu-id="4fa67-103">Get plannerRosterMember</span><span class="sxs-lookup"><span data-stu-id="4fa67-103">Get plannerRosterMember</span></span>
<span data-ttu-id="4fa67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fa67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fa67-105">Чтение свойств и связей объекта [plannerRosterMember.](../resources/plannerrostermember.md)</span><span class="sxs-lookup"><span data-stu-id="4fa67-105">Read the properties and relationships of a [plannerRosterMember](../resources/plannerrostermember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fa67-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fa67-106">Permissions</span></span>
<span data-ttu-id="4fa67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fa67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fa67-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fa67-109">Permission type</span></span>|<span data-ttu-id="4fa67-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fa67-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fa67-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fa67-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4fa67-112">Tasks.Read, Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fa67-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="4fa67-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fa67-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fa67-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa67-114">Not supported.</span></span>|
|<span data-ttu-id="4fa67-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fa67-115">Application</span></span>|<span data-ttu-id="4fa67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fa67-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fa67-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fa67-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/rosters/{plannerRosterId}/members/{plannerRosterMemberId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4fa67-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4fa67-118">Optional query parameters</span></span>
<span data-ttu-id="4fa67-119">Этот метод поддерживает только следующие параметры запроса OData:</span><span class="sxs-lookup"><span data-stu-id="4fa67-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="4fa67-120">$select</span><span class="sxs-lookup"><span data-stu-id="4fa67-120">$select</span></span>

<span data-ttu-id="4fa67-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4fa67-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fa67-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fa67-122">Request headers</span></span>
|<span data-ttu-id="4fa67-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4fa67-123">Name</span></span>|<span data-ttu-id="4fa67-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4fa67-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4fa67-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fa67-125">Authorization</span></span>|<span data-ttu-id="4fa67-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fa67-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fa67-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4fa67-128">Request body</span></span>
<span data-ttu-id="4fa67-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fa67-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4fa67-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4fa67-130">Response</span></span>

<span data-ttu-id="4fa67-131">В случае успеха этот метод возвращает код отклика и объект `200 OK` [plannerRosterMember](../resources/plannerrostermember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4fa67-131">If successful, this method returns a `200 OK` response code and a [plannerRosterMember](../resources/plannerrostermember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4fa67-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="4fa67-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4fa67-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fa67-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4fa67-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fa67-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerrostermember"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/rosters/523a9d5a-f9d5-45c1-929f-b8525393515c/members/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38
```
# <a name="c"></a>[<span data-ttu-id="4fa67-135">C#</span><span class="sxs-lookup"><span data-stu-id="4fa67-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerrostermember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4fa67-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fa67-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerrostermember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fa67-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fa67-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerrostermember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4fa67-138">Java</span><span class="sxs-lookup"><span data-stu-id="4fa67-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerrostermember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4fa67-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fa67-139">Response</span></span>
<span data-ttu-id="4fa67-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4fa67-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRosterMember"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerRosterMember",
  "id": "670095cd-95cd-6700-cd95-0067cd950067",
  "userId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
  "tenantId": "7084c257-c1b7-4286-98b0-20ea7b5c1319",
  "roles": [
  ]
}
```

