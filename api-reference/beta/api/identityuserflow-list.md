---
title: Список Усерфловс
description: Получение списка объектов Усерфлов.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 585353891219f47666b980a532cd8a7d3dea3918
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938600"
---
# <a name="list-userflows"></a><span data-ttu-id="56367-103">Список Усерфловс</span><span class="sxs-lookup"><span data-stu-id="56367-103">List userFlows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56367-104">Получение списка [усерфловс](../resources/identityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="56367-104">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="56367-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56367-105">Permissions</span></span>

<span data-ttu-id="56367-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56367-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56367-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56367-108">Permission type</span></span>                        | <span data-ttu-id="56367-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56367-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="56367-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56367-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="56367-111">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="56367-111">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="56367-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56367-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56367-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56367-113">Not supported.</span></span> |
| <span data-ttu-id="56367-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56367-114">Application</span></span>                            | <span data-ttu-id="56367-115">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="56367-115">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56367-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56367-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="56367-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56367-117">Request headers</span></span>

| <span data-ttu-id="56367-118">Имя</span><span class="sxs-lookup"><span data-stu-id="56367-118">Name</span></span>      |<span data-ttu-id="56367-119">Описание</span><span class="sxs-lookup"><span data-stu-id="56367-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56367-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56367-120">Authorization</span></span> | <span data-ttu-id="56367-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56367-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56367-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56367-123">Request body</span></span>

<span data-ttu-id="56367-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56367-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56367-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="56367-125">Response</span></span>

<span data-ttu-id="56367-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерфлов](../resources/identityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56367-126">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56367-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="56367-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56367-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="56367-128">Request</span></span>

<span data-ttu-id="56367-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56367-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="56367-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="56367-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56367-131">C#</span><span class="sxs-lookup"><span data-stu-id="56367-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56367-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56367-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56367-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56367-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56367-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="56367-134">Response</span></span>

<span data-ttu-id="56367-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56367-135">The following is an example of the response.</span></span>

> <span data-ttu-id="56367-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56367-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "B2C_1_UserFlow1",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_userflows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
