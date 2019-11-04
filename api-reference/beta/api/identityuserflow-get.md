---
title: Получение Усерфлов
description: Получение свойств и связей объекта усерфлов.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee9bedb3fd81d638e8e7d996e1d6afe9e8ce1c64
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938630"
---
# <a name="get-userflow"></a><span data-ttu-id="ef8c0-103">Получение Усерфлов</span><span class="sxs-lookup"><span data-stu-id="ef8c0-103">Get userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef8c0-104">Получение свойств и связей для объекта [усерфлов](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="ef8c0-104">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef8c0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef8c0-105">Permissions</span></span>

<span data-ttu-id="ef8c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef8c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef8c0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef8c0-108">Permission type</span></span>                        | <span data-ttu-id="ef8c0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef8c0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ef8c0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef8c0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef8c0-111">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef8c0-111">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="ef8c0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef8c0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef8c0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef8c0-113">Not supported.</span></span> |
| <span data-ttu-id="ef8c0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef8c0-114">Application</span></span>                            | <span data-ttu-id="ef8c0-115">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef8c0-115">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef8c0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef8c0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ef8c0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef8c0-117">Request headers</span></span>

| <span data-ttu-id="ef8c0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ef8c0-118">Name</span></span>      |<span data-ttu-id="ef8c0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ef8c0-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef8c0-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef8c0-120">Authorization</span></span> | <span data-ttu-id="ef8c0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef8c0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef8c0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef8c0-123">Content-type</span></span> | <span data-ttu-id="ef8c0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef8c0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef8c0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef8c0-126">Request body</span></span>

<span data-ttu-id="ef8c0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef8c0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef8c0-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef8c0-128">Response</span></span>

<span data-ttu-id="ef8c0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [усерфлов](../resources/identityuserflow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef8c0-129">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef8c0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef8c0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef8c0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef8c0-131">Request</span></span>

<span data-ttu-id="ef8c0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef8c0-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ef8c0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef8c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef8c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef8c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef8c0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef8c0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef8c0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef8c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ef8c0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef8c0-137">Response</span></span>

<span data-ttu-id="ef8c0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef8c0-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ef8c0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef8c0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
   "suppressions": [
    "Error: get_identityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
