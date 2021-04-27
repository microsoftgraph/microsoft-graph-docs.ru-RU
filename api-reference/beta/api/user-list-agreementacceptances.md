---
title: Перечисление agreementAcceptances
description: Извлечение списка объектов agreementAcceptance пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8785d78b99b836ef32e8c85088dd7e4bb0deb374
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036340"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="7a46e-103">Перечисление agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="7a46e-103">List agreementAcceptances</span></span>

<span data-ttu-id="7a46e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a46e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a46e-105">Извлечение списка объектов [agreementAcceptance пользователя.](../resources/agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="7a46e-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a46e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a46e-106">Permissions</span></span>
<span data-ttu-id="7a46e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a46e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a46e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a46e-109">Permission type</span></span>                        | <span data-ttu-id="7a46e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a46e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a46e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a46e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a46e-112">AgreementAcceptance.Read, AgreementAcceptance.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a46e-112">AgreementAcceptance.Read, AgreementAcceptance.Read.All</span></span> |
|<span data-ttu-id="7a46e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a46e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a46e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a46e-114">Not supported.</span></span> |
|<span data-ttu-id="7a46e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a46e-115">Application</span></span>                            | <span data-ttu-id="7a46e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a46e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a46e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a46e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="7a46e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a46e-118">Request headers</span></span>
| <span data-ttu-id="7a46e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7a46e-119">Name</span></span>      |<span data-ttu-id="7a46e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7a46e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7a46e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a46e-121">Authorization</span></span> | <span data-ttu-id="7a46e-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="7a46e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a46e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a46e-123">Request body</span></span>
<span data-ttu-id="7a46e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a46e-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7a46e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a46e-125">Response</span></span>
<span data-ttu-id="7a46e-126">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов agreementAcceptance](../resources/agreementacceptance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7a46e-126">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a46e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7a46e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a46e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a46e-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a46e-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a46e-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="7a46e-130">C#</span><span class="sxs-lookup"><span data-stu-id="7a46e-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a46e-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a46e-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a46e-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a46e-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a46e-133">Java</span><span class="sxs-lookup"><span data-stu-id="7a46e-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a46e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a46e-134">Response</span></span>
><span data-ttu-id="7a46e-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7a46e-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
