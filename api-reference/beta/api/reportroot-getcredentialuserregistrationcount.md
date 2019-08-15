---
title: 'Reportroot.: Жеткредентиалусеррегистратионкаунт'
description: Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 1ec286eb86b3dbeeb5f7687b2af00a36b76348b4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411923"
---
# <a name="reportroot-getcredentialuserregistrationcount"></a><span data-ttu-id="8df13-103">Reportroot.: Жеткредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="8df13-103">reportRoot: getCredentialUserRegistrationCount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8df13-104">Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="8df13-104">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="8df13-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8df13-105">Permissions</span></span>

<span data-ttu-id="8df13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8df13-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8df13-108">Permission type</span></span>                        | <span data-ttu-id="8df13-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8df13-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8df13-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8df13-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8df13-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8df13-111">Reports.Read.All</span></span> |
| <span data-ttu-id="8df13-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8df13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8df13-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df13-113">Not supported.</span></span> |
| <span data-ttu-id="8df13-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8df13-114">Application</span></span>                            | <span data-ttu-id="8df13-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8df13-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8df13-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8df13-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUserRegistrationCount
```

## <a name="request-headers"></a><span data-ttu-id="8df13-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8df13-117">Request headers</span></span>

| <span data-ttu-id="8df13-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8df13-118">Name</span></span>          | <span data-ttu-id="8df13-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8df13-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8df13-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8df13-120">Authorization</span></span> | <span data-ttu-id="8df13-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8df13-121">Bearer {token}</span></span> |
| <span data-ttu-id="8df13-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8df13-122">Content-Type</span></span> | <span data-ttu-id="8df13-123">application/json</span><span class="sxs-lookup"><span data-stu-id="8df13-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8df13-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8df13-124">Request body</span></span>

<span data-ttu-id="8df13-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8df13-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8df13-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8df13-126">Response</span></span>

<span data-ttu-id="8df13-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [кредентиалусеррегистратионкаунт](../resources/credentialuserregistrationcount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8df13-127">If successful, this method returns a `200 OK` response code and a new [credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8df13-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8df13-128">Examples</span></span>

<span data-ttu-id="8df13-129">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8df13-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8df13-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8df13-130">Request</span></span>

<span data-ttu-id="8df13-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8df13-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8df13-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8df13-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialuserregistrationcount"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getCredentialUserRegistrationCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8df13-133">C#</span><span class="sxs-lookup"><span data-stu-id="8df13-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialuserregistrationcount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8df13-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8df13-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialuserregistrationcount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8df13-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8df13-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialuserregistrationcount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8df13-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8df13-136">Response</span></span>

<span data-ttu-id="8df13-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8df13-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8df13-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8df13-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8df13-139">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8df13-139">All the properties are returned from an actual call.</span></span>

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
