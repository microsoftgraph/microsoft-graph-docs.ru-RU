---
title: 'Reportroot.: Жеткредентиалусеррегистратионкаунт'
description: Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: db1324efe4148deefeb83f662ab363f0671d9da4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874118"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="b9f53-103">Reportroot.: Жеткредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="b9f53-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9f53-104">Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="b9f53-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9f53-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f53-105">Permissions</span></span>

<span data-ttu-id="b9f53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9f53-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f53-108">Permission type</span></span>                        | <span data-ttu-id="b9f53-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9f53-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9f53-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f53-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9f53-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f53-111">Reports.Read.All</span></span> |
| <span data-ttu-id="b9f53-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9f53-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f53-113">Not supported.</span></span> |
| <span data-ttu-id="b9f53-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9f53-114">Application</span></span>                            | <span data-ttu-id="b9f53-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f53-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9f53-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f53-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="b9f53-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9f53-117">Request headers</span></span>

| <span data-ttu-id="b9f53-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b9f53-118">Name</span></span>          | <span data-ttu-id="b9f53-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f53-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b9f53-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9f53-120">Authorization</span></span> | <span data-ttu-id="b9f53-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b9f53-121">Bearer {token}</span></span> |
| <span data-ttu-id="b9f53-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9f53-122">Content-Type</span></span> | <span data-ttu-id="b9f53-123">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f53-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9f53-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9f53-124">Request body</span></span>

<span data-ttu-id="b9f53-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9f53-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9f53-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f53-126">Response</span></span>

<span data-ttu-id="b9f53-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [кредентиалусеррегистратионкаунт](../resources/credentialuserregistrationcount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9f53-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9f53-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9f53-128">Examples</span></span>

<span data-ttu-id="b9f53-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b9f53-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b9f53-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9f53-130">Request</span></span>

<span data-ttu-id="b9f53-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9f53-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b9f53-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9f53-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b9f53-133">C#</span><span class="sxs-lookup"><span data-stu-id="b9f53-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9f53-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b9f53-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b9f53-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b9f53-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b9f53-136">Java</span><span class="sxs-lookup"><span data-stu-id="b9f53-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialuserregistrationcount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9f53-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f53-137">Response</span></span>

<span data-ttu-id="b9f53-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f53-138">The following is an example of the response.</span></span>

> <span data-ttu-id="b9f53-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b9f53-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b9f53-140">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b9f53-140">All the properties are returned from an actual call.</span></span>

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
