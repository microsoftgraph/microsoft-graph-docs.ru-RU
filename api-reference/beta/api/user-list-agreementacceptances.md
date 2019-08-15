---
title: Перечисление agreementAcceptances
description: Получение списка объектов agreementAcceptance пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d64915ee5e61521176a705ac5877ee449a01d60e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409004"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="f4e3a-103">Перечисление agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="f4e3a-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4e3a-104">Получение списка объектов [agreementAcceptance](../resources/agreementacceptance.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4e3a-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4e3a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4e3a-105">Permissions</span></span>
<span data-ttu-id="f4e3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4e3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4e3a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4e3a-108">Permission type</span></span>                        | <span data-ttu-id="f4e3a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4e3a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4e3a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4e3a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4e3a-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="f4e3a-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="f4e3a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4e3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4e3a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4e3a-113">Not supported.</span></span> |
|<span data-ttu-id="f4e3a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4e3a-114">Application</span></span>                            | <span data-ttu-id="f4e3a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4e3a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4e3a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4e3a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="f4e3a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4e3a-117">Request headers</span></span>
| <span data-ttu-id="f4e3a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f4e3a-118">Name</span></span>      |<span data-ttu-id="f4e3a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f4e3a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4e3a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4e3a-120">Authorization</span></span> | <span data-ttu-id="f4e3a-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f4e3a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4e3a-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4e3a-122">Request body</span></span>
<span data-ttu-id="f4e3a-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4e3a-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f4e3a-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4e3a-124">Response</span></span>
<span data-ttu-id="f4e3a-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [agreementAcceptance](../resources/agreementacceptance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4e3a-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f4e3a-126">Пример</span><span class="sxs-lookup"><span data-stu-id="f4e3a-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4e3a-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4e3a-127">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f4e3a-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4e3a-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4e3a-129">C#</span><span class="sxs-lookup"><span data-stu-id="f4e3a-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4e3a-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4e3a-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4e3a-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f4e3a-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f4e3a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4e3a-132">Response</span></span>
><span data-ttu-id="f4e3a-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4e3a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
