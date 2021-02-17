---
title: Get plannerRoster
description: Чтение свойств и связей объекта plannerRoster.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 49aa19c85cea3d103b6338a46ccd605c89759e95
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271901"
---
# <a name="get-plannerroster"></a><span data-ttu-id="a0df4-103">Get plannerRoster</span><span class="sxs-lookup"><span data-stu-id="a0df4-103">Get plannerRoster</span></span>
<span data-ttu-id="a0df4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0df4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0df4-105">Чтение свойств и связей объекта [plannerRoster.](../resources/plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="a0df4-105">Read the properties and relationships of a [plannerRoster](../resources/plannerroster.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0df4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0df4-106">Permissions</span></span>
<span data-ttu-id="a0df4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0df4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0df4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0df4-109">Permission type</span></span>|<span data-ttu-id="a0df4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0df4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0df4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0df4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0df4-112">Tasks.Read, Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0df4-112">Tasks.Read, Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a0df4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0df4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0df4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0df4-114">Not supported.</span></span>|
|<span data-ttu-id="a0df4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0df4-115">Application</span></span>|<span data-ttu-id="a0df4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0df4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0df4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0df4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/rosters/{plannerRosterId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0df4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0df4-118">Optional query parameters</span></span>
<span data-ttu-id="a0df4-119">Этот метод поддерживает только следующие параметры запроса OData:</span><span class="sxs-lookup"><span data-stu-id="a0df4-119">This method only supports following OData query parameters:</span></span>

- <span data-ttu-id="a0df4-120">$expand</span><span class="sxs-lookup"><span data-stu-id="a0df4-120">$expand</span></span>

<span data-ttu-id="a0df4-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a0df4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0df4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0df4-122">Request headers</span></span>
|<span data-ttu-id="a0df4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a0df4-123">Name</span></span>|<span data-ttu-id="a0df4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a0df4-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a0df4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0df4-125">Authorization</span></span>|<span data-ttu-id="a0df4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0df4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0df4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0df4-128">Request body</span></span>
<span data-ttu-id="a0df4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0df4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0df4-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0df4-130">Response</span></span>

<span data-ttu-id="a0df4-131">В случае успеха этот метод возвращает код отклика и объект `200 OK` [plannerRoster](../resources/plannerroster.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0df4-131">If successful, this method returns a `200 OK` response code and a [plannerRoster](../resources/plannerroster.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0df4-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="a0df4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0df4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0df4-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a0df4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0df4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerroster"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/rosters/6519868f-868f-6519-8f86-19658f861965
```
# <a name="c"></a>[<span data-ttu-id="a0df4-135">C#</span><span class="sxs-lookup"><span data-stu-id="a0df4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerroster-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0df4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0df4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerroster-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0df4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0df4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerroster-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0df4-138">Java</span><span class="sxs-lookup"><span data-stu-id="a0df4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerroster-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a0df4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0df4-139">Response</span></span>
<span data-ttu-id="a0df4-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a0df4-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerRoster"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.plannerRoster",
    "id": "6519868f-868f-6519-8f86-19658f861965"
  }
}
```

