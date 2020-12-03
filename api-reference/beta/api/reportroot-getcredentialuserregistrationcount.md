---
title: 'Reportroot.: Жеткредентиалусеррегистратионкаунт'
description: Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 8fd2b2d950055eb778242664b95e0eaafe95dbc9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523058"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="e9628-103">Reportroot.: Жеткредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="e9628-103">reportRoot: getCredentialUserRegistrationCount</span></span>

<span data-ttu-id="e9628-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9628-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9628-105">Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="e9628-105">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9628-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9628-106">Permissions</span></span>

<span data-ttu-id="e9628-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9628-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9628-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9628-109">Permission type</span></span>                        | <span data-ttu-id="e9628-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9628-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9628-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9628-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9628-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9628-112">Reports.Read.All</span></span> |
| <span data-ttu-id="e9628-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9628-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9628-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9628-114">Not supported.</span></span> |
| <span data-ttu-id="e9628-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9628-115">Application</span></span>                            | <span data-ttu-id="e9628-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9628-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9628-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9628-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="e9628-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9628-118">Request headers</span></span>

| <span data-ttu-id="e9628-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e9628-119">Name</span></span>          | <span data-ttu-id="e9628-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e9628-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e9628-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9628-121">Authorization</span></span> | <span data-ttu-id="e9628-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e9628-122">Bearer {token}</span></span> |
| <span data-ttu-id="e9628-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9628-123">Content-Type</span></span> | <span data-ttu-id="e9628-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e9628-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9628-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9628-125">Request body</span></span>

<span data-ttu-id="e9628-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9628-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9628-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9628-127">Response</span></span>

<span data-ttu-id="e9628-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [кредентиалусеррегистратионкаунт](../resources/credentialuserregistrationcount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9628-128">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9628-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="e9628-129">Examples</span></span>

<span data-ttu-id="e9628-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e9628-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e9628-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9628-131">Request</span></span>

<span data-ttu-id="e9628-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9628-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9628-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9628-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="c"></a>[<span data-ttu-id="e9628-134">C#</span><span class="sxs-lookup"><span data-stu-id="e9628-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9628-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9628-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9628-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9628-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9628-137">Java</span><span class="sxs-lookup"><span data-stu-id="e9628-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialuserregistrationcount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9628-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9628-138">Response</span></span>

<span data-ttu-id="e9628-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e9628-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e9628-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e9628-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e9628-141">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9628-141">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationCount)",
  "value": [
    {
      "id" : "id-value",
      "totalUserCount" : 23123,
      "userRegistrationCounts" :
      [
        { "userRegistrationStatus":"registered", 
          "userRegistationCount": 23423 }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUserRegistrationCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


