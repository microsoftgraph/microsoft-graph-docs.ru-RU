---
title: Список rosterPlans
description: Получите ресурсы plannerPlan из свойства навигации rosterPlans.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 199697f7cd3ee050caac983e9822007cdc38a557
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272487"
---
# <a name="list-rosterplans"></a><span data-ttu-id="d2747-103">Список rosterPlans</span><span class="sxs-lookup"><span data-stu-id="d2747-103">List rosterPlans</span></span>
<span data-ttu-id="d2747-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2747-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2747-105">Получите список [plannerPlans,](../resources/plannerplan.md) содержащихся в [планировщикеRosters,](../resources/plannerroster.md) участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="d2747-105">Get the list of [plannerPlans](../resources/plannerplan.md) that are contained by the [plannerRosters](../resources/plannerroster.md) of which the user is a member.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2747-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2747-106">Permissions</span></span>
<span data-ttu-id="d2747-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2747-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2747-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2747-109">Permission type</span></span>|<span data-ttu-id="d2747-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2747-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2747-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2747-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2747-112">Tasks.Read, Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2747-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="d2747-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2747-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2747-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2747-114">Not supported.</span></span>|
|<span data-ttu-id="d2747-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2747-115">Application</span></span>|<span data-ttu-id="d2747-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2747-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2747-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2747-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/planner/rosterPlans
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2747-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2747-118">Optional query parameters</span></span>
<span data-ttu-id="d2747-119">Этот метод поддерживает только следующие параметры запроса OData:</span><span class="sxs-lookup"><span data-stu-id="d2747-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="d2747-120">$select</span><span class="sxs-lookup"><span data-stu-id="d2747-120">$select</span></span>

<span data-ttu-id="d2747-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d2747-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2747-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2747-122">Request headers</span></span>
|<span data-ttu-id="d2747-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d2747-123">Name</span></span>|<span data-ttu-id="d2747-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d2747-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2747-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2747-125">Authorization</span></span>|<span data-ttu-id="d2747-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2747-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2747-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2747-128">Request body</span></span>
<span data-ttu-id="d2747-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2747-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2747-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2747-130">Response</span></span>

<span data-ttu-id="d2747-131">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [plannerPlan](../resources/plannerplan.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2747-131">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2747-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2747-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2747-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2747-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d2747-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2747-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_plannerplan"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/planner/rosterPlans
```
# <a name="c"></a>[<span data-ttu-id="d2747-135">C#</span><span class="sxs-lookup"><span data-stu-id="d2747-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-plannerplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2747-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2747-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-plannerplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2747-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2747-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-plannerplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2747-138">Java</span><span class="sxs-lookup"><span data-stu-id="d2747-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-plannerplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d2747-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2747-139">Response</span></span>
<span data-ttu-id="d2747-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d2747-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.plannerPlan)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerPlan",
      "id": "c6442b38-2b38-c644-382b-44c6382b44c6",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "title": "Test plan",
      "container": {
        "@odata.type": "microsoft.graph.plannerPlanContainer",
        "url": "https://graph.microsoft.com/beta/planner/rosters/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
        "containerId": "5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38",
        "type": "roster"
      }
    }
  ]
}
```

