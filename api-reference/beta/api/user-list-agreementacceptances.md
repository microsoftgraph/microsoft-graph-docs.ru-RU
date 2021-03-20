---
title: Перечисление agreementAcceptances
description: Извлечение списка объектов agreementAcceptance пользователя.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 178e6afe9b9bd62e1f921f6ddc6c3c9148c57cb9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943700"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="a818c-103">Перечисление agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="a818c-103">List agreementAcceptances</span></span>

<span data-ttu-id="a818c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a818c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a818c-105">Извлечение списка объектов [agreementAcceptance пользователя.](../resources/agreementacceptance.md)</span><span class="sxs-lookup"><span data-stu-id="a818c-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="a818c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a818c-106">Permissions</span></span>
<span data-ttu-id="a818c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a818c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a818c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a818c-109">Permission type</span></span>                        | <span data-ttu-id="a818c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a818c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a818c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a818c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a818c-112">AgreementAcceptance.Read, AgreementAcceptance.Read.All</span><span class="sxs-lookup"><span data-stu-id="a818c-112">AgreementAcceptance.Read, AgreementAcceptance.Read.All</span></span> |
|<span data-ttu-id="a818c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a818c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a818c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a818c-114">Not supported.</span></span> |
|<span data-ttu-id="a818c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a818c-115">Application</span></span>                            | <span data-ttu-id="a818c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a818c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a818c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a818c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="a818c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a818c-118">Request headers</span></span>
| <span data-ttu-id="a818c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a818c-119">Name</span></span>      |<span data-ttu-id="a818c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a818c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a818c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a818c-121">Authorization</span></span> | <span data-ttu-id="a818c-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a818c-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a818c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a818c-123">Request body</span></span>
<span data-ttu-id="a818c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a818c-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a818c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a818c-125">Response</span></span>
<span data-ttu-id="a818c-126">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов agreementAcceptance](../resources/agreementacceptance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a818c-126">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a818c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a818c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a818c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a818c-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a818c-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="a818c-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="a818c-130">C#</span><span class="sxs-lookup"><span data-stu-id="a818c-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a818c-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a818c-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a818c-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a818c-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a818c-133">Java</span><span class="sxs-lookup"><span data-stu-id="a818c-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a818c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a818c-134">Response</span></span>
><span data-ttu-id="a818c-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a818c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
