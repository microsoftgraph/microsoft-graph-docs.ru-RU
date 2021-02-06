---
title: Список credentialUserRegistrationDetails
description: Получите список объектов credentialUserRegistrationDetails для данного клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: bf6e99722c44ff0054869056be09314d6befac59
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136670"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="8b21a-103">Список credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="8b21a-103">List credentialUserRegistrationDetails</span></span>

<span data-ttu-id="8b21a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b21a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b21a-105">Получите список объектов [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="8b21a-105">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b21a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b21a-106">Permissions</span></span>

<span data-ttu-id="8b21a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b21a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b21a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b21a-109">Permission type</span></span>                        | <span data-ttu-id="8b21a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b21a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b21a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b21a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b21a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b21a-112">Reports.Read.All</span></span> |
| <span data-ttu-id="8b21a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b21a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b21a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b21a-114">Not supported.</span></span> |
| <span data-ttu-id="8b21a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b21a-115">Application</span></span>                            | <span data-ttu-id="8b21a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b21a-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b21a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b21a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b21a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b21a-118">Optional query parameters</span></span>

<span data-ttu-id="8b21a-119">Эта функция поддерживает необязательный параметр запроса OData **$filter.**</span><span class="sxs-lookup"><span data-stu-id="8b21a-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="8b21a-120">Вы можете **применить $filter** к одному или более из следующих свойств ресурса [credentialUserRegistrationDetails.](../resources/credentialuserregistrationdetails.md)</span><span class="sxs-lookup"><span data-stu-id="8b21a-120">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="8b21a-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b21a-121">Properties</span></span> | <span data-ttu-id="8b21a-122">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="8b21a-122">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="8b21a-123">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8b21a-123">userDisplayName</span></span> | <span data-ttu-id="8b21a-124">Фильтрация по имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b21a-124">Filter by user name.</span></span> <span data-ttu-id="8b21a-125">Пример: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="8b21a-125">For example: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="8b21a-126">Поддерживаемые операторы фильтра: `eq` и `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="8b21a-126">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="8b21a-127">Поддерживается безчувствительности к делу.</span><span class="sxs-lookup"><span data-stu-id="8b21a-127">Supports case insensitive.</span></span> |
| <span data-ttu-id="8b21a-128">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b21a-128">userPrincipalName</span></span> | <span data-ttu-id="8b21a-129">Фильтрация по имени основного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b21a-129">Filter by user principal name.</span></span> <span data-ttu-id="8b21a-130">Пример: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="8b21a-130">For example: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="8b21a-131">Поддерживаемые операторы фильтра: `eq` и `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="8b21a-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="8b21a-132">Поддерживается безчувствительности к делу.</span><span class="sxs-lookup"><span data-stu-id="8b21a-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="8b21a-133">authMethods</span><span class="sxs-lookup"><span data-stu-id="8b21a-133">authMethods</span></span> | <span data-ttu-id="8b21a-134">Фильтрация по методам проверки подлинности, используемым во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="8b21a-134">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="8b21a-135">Пример: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span><span class="sxs-lookup"><span data-stu-id="8b21a-135">For example: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="8b21a-136">Поддерживаемые операторы фильтра: `eq` .</span><span class="sxs-lookup"><span data-stu-id="8b21a-136">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="8b21a-137">isRegistered</span><span class="sxs-lookup"><span data-stu-id="8b21a-137">isRegistered</span></span> | <span data-ttu-id="8b21a-138">Фильтрация для пользователей, которые зарегистрировались для самостоятельного сброса пароля (SSPR).</span><span class="sxs-lookup"><span data-stu-id="8b21a-138">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="8b21a-139">Пример: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="8b21a-139">For example: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="8b21a-140">Поддерживаемые операторы фильтра: `eq` .</span><span class="sxs-lookup"><span data-stu-id="8b21a-140">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="8b21a-141">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8b21a-141">isEnabled</span></span> | <span data-ttu-id="8b21a-142">Фильтрация для пользователей, для которых включена SSPR.</span><span class="sxs-lookup"><span data-stu-id="8b21a-142">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="8b21a-143">Пример: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span><span class="sxs-lookup"><span data-stu-id="8b21a-143">For example: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="8b21a-144">Поддерживаемые операторы filtter: `eq` .</span><span class="sxs-lookup"><span data-stu-id="8b21a-144">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="8b21a-145">isCapable</span><span class="sxs-lookup"><span data-stu-id="8b21a-145">isCapable</span></span> | <span data-ttu-id="8b21a-146">Фильтрация для пользователей, которые готовы выполнить сброс пароля или многофакторную проверку подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="8b21a-146">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="8b21a-147">Пример: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span><span class="sxs-lookup"><span data-stu-id="8b21a-147">For example: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="8b21a-148">Поддерживаемые операторы фильтров: `eq`</span><span class="sxs-lookup"><span data-stu-id="8b21a-148">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="8b21a-149">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="8b21a-149">isMfaRegistered</span></span> | <span data-ttu-id="8b21a-150">Фильтрация для пользователей, зарегистрированных на MFA.</span><span class="sxs-lookup"><span data-stu-id="8b21a-150">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="8b21a-151">Пример: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="8b21a-151">For example: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="8b21a-152">Поддерживаемые операторы фильтра: `eq` .</span><span class="sxs-lookup"><span data-stu-id="8b21a-152">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="8b21a-153">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b21a-153">Request headers</span></span>

| <span data-ttu-id="8b21a-154">Имя</span><span class="sxs-lookup"><span data-stu-id="8b21a-154">Name</span></span>      |<span data-ttu-id="8b21a-155">Описание</span><span class="sxs-lookup"><span data-stu-id="8b21a-155">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b21a-156">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b21a-156">Authorization</span></span> | <span data-ttu-id="8b21a-157">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8b21a-157">Bearer {token}</span></span> |
| <span data-ttu-id="8b21a-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b21a-158">Content-Type</span></span> | <span data-ttu-id="8b21a-159">application/json</span><span class="sxs-lookup"><span data-stu-id="8b21a-159">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b21a-160">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b21a-160">Request body</span></span>

<span data-ttu-id="8b21a-161">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b21a-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b21a-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b21a-162">Response</span></span>

<span data-ttu-id="8b21a-163">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b21a-163">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b21a-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="8b21a-164">Examples</span></span>

<span data-ttu-id="8b21a-165">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8b21a-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8b21a-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b21a-166">Request</span></span>

<span data-ttu-id="8b21a-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b21a-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b21a-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b21a-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[<span data-ttu-id="8b21a-169">C#</span><span class="sxs-lookup"><span data-stu-id="8b21a-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b21a-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b21a-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b21a-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b21a-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b21a-172">Java</span><span class="sxs-lookup"><span data-stu-id="8b21a-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b21a-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b21a-173">Response</span></span>

<span data-ttu-id="8b21a-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b21a-174">The following is an example of the response.</span></span>

> <span data-ttu-id="8b21a-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8b21a-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8b21a-176">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8b21a-176">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationDetails)",
  "value":[
    {
      "id" : "id-value",
      "userPrincipalName":"userPrincipalName",
      "userDisplayName": "userDisplayName-value",
      "authMethods": ["email", "mobileSMS"],
      "isRegistered" : false,
      "isEnabled" : true,
      "isCapable" : false,
      "isMfaRegistered" : true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List credentialUserRegistrationDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


