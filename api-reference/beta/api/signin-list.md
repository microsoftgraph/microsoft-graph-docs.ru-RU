---
title: Перечисление входов
doc_type: apiPageType
description: Получение списка входов пользователей в клиенте Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5fa97184a4858d3b8fee7b537310cc09270a749b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938367"
---
# <a name="list-signins"></a><span data-ttu-id="16fdc-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="16fdc-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16fdc-104">Получение списка объектов [SignIn](../resources/signin.md) .</span><span class="sxs-lookup"><span data-stu-id="16fdc-104">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="16fdc-105">В этом списке содержатся входы пользователей для клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="16fdc-105">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="16fdc-106">Входы, в которых имя пользователя и пароль передаются в составе маркера авторизации, а успешные Федеративные входы в систему в данный момент включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="16fdc-106">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="16fdc-107">Первыми возвращаются последние входные.</span><span class="sxs-lookup"><span data-stu-id="16fdc-107">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="16fdc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16fdc-108">Permissions</span></span>

<span data-ttu-id="16fdc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16fdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16fdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16fdc-111">Permission type</span></span> | <span data-ttu-id="16fdc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16fdc-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="16fdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16fdc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="16fdc-114">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="16fdc-114">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="16fdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16fdc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16fdc-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="16fdc-116">Not supported</span></span> |
| <span data-ttu-id="16fdc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16fdc-117">Application</span></span> | <span data-ttu-id="16fdc-118">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="16fdc-118">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="16fdc-119">Кроме того, приложения должны быть должным образом зарегистрированы в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="16fdc-119">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="16fdc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16fdc-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16fdc-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16fdc-121">Optional query parameters</span></span>

<span data-ttu-id="16fdc-122">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="16fdc-122">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="16fdc-123">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="16fdc-123">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="16fdc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="16fdc-124">Name</span></span> | <span data-ttu-id="16fdc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="16fdc-125">Description</span></span> | <span data-ttu-id="16fdc-126">Пример</span><span class="sxs-lookup"><span data-stu-id="16fdc-126">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="16fdc-127">$filter</span><span class="sxs-lookup"><span data-stu-id="16fdc-127">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)| <span data-ttu-id="16fdc-128">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="16fdc-128">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="16fdc-129">$top</span><span class="sxs-lookup"><span data-stu-id="16fdc-129">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter) | <span data-ttu-id="16fdc-130">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="16fdc-130">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="16fdc-131">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="16fdc-131">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter) | <span data-ttu-id="16fdc-132">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="16fdc-132">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="16fdc-133">Атрибуты, поддерживаемые параметром $filter</span><span class="sxs-lookup"><span data-stu-id="16fdc-133">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="16fdc-134">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="16fdc-134">Attribute Name</span></span> | <span data-ttu-id="16fdc-135">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="16fdc-135">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="16fdc-136">id</span><span class="sxs-lookup"><span data-stu-id="16fdc-136">id</span></span> | <span data-ttu-id="16fdc-137">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-137">eq</span></span> |
| <span data-ttu-id="16fdc-138">userId</span><span class="sxs-lookup"><span data-stu-id="16fdc-138">userId</span></span> | <span data-ttu-id="16fdc-139">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-139">eq</span></span> |
| <span data-ttu-id="16fdc-140">appId</span><span class="sxs-lookup"><span data-stu-id="16fdc-140">appId</span></span> | <span data-ttu-id="16fdc-141">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-141">eq</span></span> |
| <span data-ttu-id="16fdc-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16fdc-142">createdDateTime</span></span> | <span data-ttu-id="16fdc-143">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="16fdc-143">eq, le, ge</span></span> |
| <span data-ttu-id="16fdc-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="16fdc-144">userDisplayName</span></span> | <span data-ttu-id="16fdc-145">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-145">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="16fdc-146">userPrincipalName</span></span> | <span data-ttu-id="16fdc-147">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-147">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="16fdc-148">appDisplayName</span></span> | <span data-ttu-id="16fdc-149">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-149">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-150">ipAddress</span><span class="sxs-lookup"><span data-stu-id="16fdc-150">ipAddress</span></span> | <span data-ttu-id="16fdc-151">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-151">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-152">location/city</span><span class="sxs-lookup"><span data-stu-id="16fdc-152">location/city</span></span> | <span data-ttu-id="16fdc-153">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-153">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-154">location/state</span><span class="sxs-lookup"><span data-stu-id="16fdc-154">location/state</span></span> | <span data-ttu-id="16fdc-155">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-155">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-156">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="16fdc-156">location/countryOrRegion</span></span> | <span data-ttu-id="16fdc-157">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-157">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-158">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="16fdc-158">status/errorCode</span></span> | <span data-ttu-id="16fdc-159">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-159">eq</span></span> |
| <span data-ttu-id="16fdc-160">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="16fdc-160">initiatedBy/user/id</span></span> | <span data-ttu-id="16fdc-161">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-161">eq</span></span> |
| <span data-ttu-id="16fdc-162">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="16fdc-162">initiatedBy/user/displayName</span></span> | <span data-ttu-id="16fdc-163">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-163">eq</span></span> |
| <span data-ttu-id="16fdc-164">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="16fdc-164">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="16fdc-165">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-165">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-166">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="16fdc-166">clientAppUsed</span></span> | <span data-ttu-id="16fdc-167">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-167">eq</span></span> |
| <span data-ttu-id="16fdc-168">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="16fdc-168">conditionalAccessStatus</span></span> | <span data-ttu-id="16fdc-169">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-169">eq</span></span> |
| <span data-ttu-id="16fdc-170">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="16fdc-170">deviceDetail/browser</span></span> | <span data-ttu-id="16fdc-171">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-171">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-172">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="16fdc-172">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="16fdc-173">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-173">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-174">correlationId</span><span class="sxs-lookup"><span data-stu-id="16fdc-174">correlationId</span></span> | <span data-ttu-id="16fdc-175">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-175">eq</span></span> |
| <span data-ttu-id="16fdc-176">riskDetail</span><span class="sxs-lookup"><span data-stu-id="16fdc-176">riskDetail</span></span> | <span data-ttu-id="16fdc-177">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-177">eq</span></span> |
| <span data-ttu-id="16fdc-178">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="16fdc-178">riskLevelAggregated</span></span> | <span data-ttu-id="16fdc-179">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-179">eq</span></span> |
| <span data-ttu-id="16fdc-180">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="16fdc-180">riskLevelDuringSignIn</span></span> | <span data-ttu-id="16fdc-181">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-181">eq</span></span> |
| <span data-ttu-id="16fdc-182">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="16fdc-182">riskEventTypes</span></span> | <span data-ttu-id="16fdc-183">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-183">eq</span></span> |
| <span data-ttu-id="16fdc-184">riskState</span><span class="sxs-lookup"><span data-stu-id="16fdc-184">riskState</span></span> | <span data-ttu-id="16fdc-185">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-185">eq</span></span> |
| <span data-ttu-id="16fdc-186">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="16fdc-186">originalRequestId</span></span> | <span data-ttu-id="16fdc-187">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-187">eq</span></span> |
| <span data-ttu-id="16fdc-188">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="16fdc-188">tokenIssuerName</span></span> | <span data-ttu-id="16fdc-189">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-189">eq</span></span> |
| <span data-ttu-id="16fdc-190">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="16fdc-190">tokenIssuerType</span></span> | <span data-ttu-id="16fdc-191">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-191">eq</span></span> |
| <span data-ttu-id="16fdc-192">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="16fdc-192">resourceDisplayName</span></span> | <span data-ttu-id="16fdc-193">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-193">eq</span></span> |
| <span data-ttu-id="16fdc-194">resourceId</span><span class="sxs-lookup"><span data-stu-id="16fdc-194">resourceId</span></span> | <span data-ttu-id="16fdc-195">eq</span><span class="sxs-lookup"><span data-stu-id="16fdc-195">eq</span></span> |
| <span data-ttu-id="16fdc-196">сервицепринЦипалид</span><span class="sxs-lookup"><span data-stu-id="16fdc-196">servicePrincipalId</span></span> | <span data-ttu-id="16fdc-197">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-197">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-198">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="16fdc-198">servicePrincipalName</span></span> | <span data-ttu-id="16fdc-199">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-199">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-200">userAgent</span><span class="sxs-lookup"><span data-stu-id="16fdc-200">userAgent</span></span> | <span data-ttu-id="16fdc-201">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-201">eq, startswith</span></span> |
| <span data-ttu-id="16fdc-202">алтернатесигниннаме</span><span class="sxs-lookup"><span data-stu-id="16fdc-202">alternateSignInName</span></span> | <span data-ttu-id="16fdc-203">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="16fdc-203">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="16fdc-204">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16fdc-204">Request headers</span></span>

| <span data-ttu-id="16fdc-205">Имя</span><span class="sxs-lookup"><span data-stu-id="16fdc-205">Name</span></span>      |<span data-ttu-id="16fdc-206">Описание</span><span class="sxs-lookup"><span data-stu-id="16fdc-206">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16fdc-207">Authorization</span><span class="sxs-lookup"><span data-stu-id="16fdc-207">Authorization</span></span> | <span data-ttu-id="16fdc-208">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="16fdc-208">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="16fdc-209">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16fdc-209">Request body</span></span>

<span data-ttu-id="16fdc-210">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16fdc-210">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16fdc-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="16fdc-211">Response</span></span>

<span data-ttu-id="16fdc-212">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16fdc-212">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16fdc-213">Примеры</span><span class="sxs-lookup"><span data-stu-id="16fdc-213">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="16fdc-214">Пример 1: пользователь подписывается с помощью MFA, который активируется политикой условного доступа.</span><span class="sxs-lookup"><span data-stu-id="16fdc-214">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="16fdc-215">Основной способ проверки подлинности — Фидо.</span><span class="sxs-lookup"><span data-stu-id="16fdc-215">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="16fdc-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="16fdc-216">Request</span></span>

<span data-ttu-id="16fdc-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16fdc-217">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="16fdc-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="16fdc-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16fdc-219">C#</span><span class="sxs-lookup"><span data-stu-id="16fdc-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16fdc-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16fdc-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16fdc-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16fdc-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="16fdc-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="16fdc-222">Response</span></span>

<span data-ttu-id="16fdc-223">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16fdc-223">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"FIDO2",
          "authenticationMethodDetail":"1G54395783",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        },
        {
          "authenticationStepDateTime":"2018-11-06T18:48:12.94725647Z",
          "authenticationMethod":"Claim in access token",
          "authenticationMethodDetail":null,
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"MFA"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"applied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="16fdc-224">Пример 2: пользователь входит только с основной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="16fdc-224">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="16fdc-225">Первичная проверка подлинности осуществляется с помощью облачного пароля.</span><span class="sxs-lookup"><span data-stu-id="16fdc-225">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="16fdc-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="16fdc-226">Request</span></span>

<span data-ttu-id="16fdc-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16fdc-227">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```

#### <a name="response"></a><span data-ttu-id="16fdc-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="16fdc-228">Response</span></span>

<span data-ttu-id="16fdc-229">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="16fdc-229">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"b01b1726-0147-425e-a7f7-21f252050400",
      "createdDateTime":"2018-11-06T18:48:33.8527147Z",
      "userDisplayName":"Jon Doe",
      "userPrincipalName":"jdoe@www.contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"207.254.19.10",
      "clientAppUsed":"Browser",
      "authenticationDetails": [ 
        {
          "authenticationStepDateTime":"2018-11-06T18:48:03.8313489Z",
          "authenticationMethod":"Password",
          "authenticationMethodDetail":"Cloud password",
          "succeeded":true,
          "authenticationStepResultDetail":"methodSucceeded",
          "authenticationStepRequirement":"Primary authentication"
        }
      ],
      "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
      "conditionalAccessStatus":"applied",
      "isInteractive":true,
      "tokenIssuerName":null,
      "tokenIssuerType":"AzureAD",
      "processingTimeInMilliseconds":100,
      "riskDetail":"none",
      "riskLevelAggregated":"none",
      "riskLevelDuringsignIn":"none",
      "riskState":"none",
      "riskEventTypes":[],
      "resourceDisplayName":"windows azure service management api",
      "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
      "status":{},
      "deviceDetail": {
        "deviceId":null,
        "displayName":null,
        "operatingSystem":"Windows 7",
        "browser":"Chrome 63.0.3239",
        "isCompliant":null,
        "isManaged":null,
        "trustType":null
      },
      "location": {
        "city":"Lithia Springs",
        "state":"Georgia",
        "countryOrRegion":"US",
        "geoCoordinates": {
          "altitude":null,
          "latitude":33.7930908203125,
          "longitude":-84.445358276367188
        }
      },
      "appliedConditionalAccessPolicies": [
        {
          "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
          "displayName":"MFA policy",
          "enforcedGrantControls": [
            "Mfa",
            "RequireCompliantDevice"
          ],
          "enforcedSessionControls":[],
          "result":"notApplied"
        },
        {
          "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
          "displayName":"PipelineTest4",
          "enforcedGrantControls":[],
          "enforcedSessionControls":[],
          "result":"notEnabled"
        }
      ],
      "authenticationProcessingDetails":[],
      "networkLocationDetails":[]
    }
  ]
}
```