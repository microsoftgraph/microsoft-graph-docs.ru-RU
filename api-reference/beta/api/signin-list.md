---
title: Перечисление входов
doc_type: apiPageType
description: Получение списка входов пользователей в клиенте Azure Active Directory.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 33b72a0361776a991f0f29675fced77379e3e215
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453270"
---
# <a name="list-signins"></a><span data-ttu-id="710a7-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="710a7-103">List signIns</span></span>

<span data-ttu-id="710a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="710a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="710a7-105">Получение списка объектов [SignIn](../resources/signin.md) .</span><span class="sxs-lookup"><span data-stu-id="710a7-105">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="710a7-106">В этом списке содержатся входы пользователей для клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="710a7-106">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="710a7-107">Входы, в которых имя пользователя и пароль передаются в составе маркера авторизации, а успешные Федеративные входы в систему в данный момент включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="710a7-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="710a7-108">Первыми возвращаются последние входные.</span><span class="sxs-lookup"><span data-stu-id="710a7-108">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="710a7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="710a7-109">Permissions</span></span>

<span data-ttu-id="710a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="710a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="710a7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="710a7-112">Permission type</span></span> | <span data-ttu-id="710a7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="710a7-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="710a7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="710a7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="710a7-115">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="710a7-115">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="710a7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="710a7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="710a7-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="710a7-117">Not supported</span></span> |
| <span data-ttu-id="710a7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="710a7-118">Application</span></span> | <span data-ttu-id="710a7-119">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="710a7-119">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="710a7-120">Кроме того, приложения должны быть должным образом зарегистрированы в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="710a7-120">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="710a7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="710a7-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="710a7-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="710a7-122">Optional query parameters</span></span>

<span data-ttu-id="710a7-123">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="710a7-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="710a7-124">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="710a7-124">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="710a7-125">Имя</span><span class="sxs-lookup"><span data-stu-id="710a7-125">Name</span></span> | <span data-ttu-id="710a7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="710a7-126">Description</span></span> | <span data-ttu-id="710a7-127">Пример</span><span class="sxs-lookup"><span data-stu-id="710a7-127">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="710a7-128">$filter</span><span class="sxs-lookup"><span data-stu-id="710a7-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)| <span data-ttu-id="710a7-129">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="710a7-129">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="710a7-130">$top</span><span class="sxs-lookup"><span data-stu-id="710a7-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter) | <span data-ttu-id="710a7-131">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="710a7-131">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="710a7-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="710a7-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter) | <span data-ttu-id="710a7-133">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="710a7-133">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="710a7-134">Атрибуты, поддерживаемые параметром $filter</span><span class="sxs-lookup"><span data-stu-id="710a7-134">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="710a7-135">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="710a7-135">Attribute Name</span></span> | <span data-ttu-id="710a7-136">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="710a7-136">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="710a7-137">id</span><span class="sxs-lookup"><span data-stu-id="710a7-137">id</span></span> | <span data-ttu-id="710a7-138">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-138">eq</span></span> |
| <span data-ttu-id="710a7-139">userId</span><span class="sxs-lookup"><span data-stu-id="710a7-139">userId</span></span> | <span data-ttu-id="710a7-140">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-140">eq</span></span> |
| <span data-ttu-id="710a7-141">appId</span><span class="sxs-lookup"><span data-stu-id="710a7-141">appId</span></span> | <span data-ttu-id="710a7-142">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-142">eq</span></span> |
| <span data-ttu-id="710a7-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="710a7-143">createdDateTime</span></span> | <span data-ttu-id="710a7-144">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="710a7-144">eq, le, ge</span></span> |
| <span data-ttu-id="710a7-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="710a7-145">userDisplayName</span></span> | <span data-ttu-id="710a7-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-146">eq, startswith</span></span> |
| <span data-ttu-id="710a7-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="710a7-147">userPrincipalName</span></span> | <span data-ttu-id="710a7-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-148">eq, startswith</span></span> |
| <span data-ttu-id="710a7-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="710a7-149">appDisplayName</span></span> | <span data-ttu-id="710a7-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-150">eq, startswith</span></span> |
| <span data-ttu-id="710a7-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="710a7-151">ipAddress</span></span> | <span data-ttu-id="710a7-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-152">eq, startswith</span></span> |
| <span data-ttu-id="710a7-153">location/city</span><span class="sxs-lookup"><span data-stu-id="710a7-153">location/city</span></span> | <span data-ttu-id="710a7-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-154">eq, startswith</span></span> |
| <span data-ttu-id="710a7-155">location/state</span><span class="sxs-lookup"><span data-stu-id="710a7-155">location/state</span></span> | <span data-ttu-id="710a7-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-156">eq, startswith</span></span> |
| <span data-ttu-id="710a7-157">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="710a7-157">location/countryOrRegion</span></span> | <span data-ttu-id="710a7-158">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-158">eq, startswith</span></span> |
| <span data-ttu-id="710a7-159">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="710a7-159">status/errorCode</span></span> | <span data-ttu-id="710a7-160">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-160">eq</span></span> |
| <span data-ttu-id="710a7-161">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="710a7-161">initiatedBy/user/id</span></span> | <span data-ttu-id="710a7-162">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-162">eq</span></span> |
| <span data-ttu-id="710a7-163">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="710a7-163">initiatedBy/user/displayName</span></span> | <span data-ttu-id="710a7-164">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-164">eq</span></span> |
| <span data-ttu-id="710a7-165">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="710a7-165">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="710a7-166">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-166">eq, startswith</span></span> |
| <span data-ttu-id="710a7-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="710a7-167">clientAppUsed</span></span> | <span data-ttu-id="710a7-168">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-168">eq</span></span> |
| <span data-ttu-id="710a7-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="710a7-169">conditionalAccessStatus</span></span> | <span data-ttu-id="710a7-170">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-170">eq</span></span> |
| <span data-ttu-id="710a7-171">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="710a7-171">deviceDetail/browser</span></span> | <span data-ttu-id="710a7-172">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-172">eq, startswith</span></span> |
| <span data-ttu-id="710a7-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="710a7-173">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="710a7-174">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-174">eq, startswith</span></span> |
| <span data-ttu-id="710a7-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="710a7-175">correlationId</span></span> | <span data-ttu-id="710a7-176">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-176">eq</span></span> |
| <span data-ttu-id="710a7-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="710a7-177">riskDetail</span></span> | <span data-ttu-id="710a7-178">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-178">eq</span></span> |
| <span data-ttu-id="710a7-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="710a7-179">riskLevelAggregated</span></span> | <span data-ttu-id="710a7-180">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-180">eq</span></span> |
| <span data-ttu-id="710a7-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="710a7-181">riskLevelDuringSignIn</span></span> | <span data-ttu-id="710a7-182">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-182">eq</span></span> |
| <span data-ttu-id="710a7-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="710a7-183">riskEventTypes</span></span> | <span data-ttu-id="710a7-184">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-184">eq</span></span> |
| <span data-ttu-id="710a7-185">riskState</span><span class="sxs-lookup"><span data-stu-id="710a7-185">riskState</span></span> | <span data-ttu-id="710a7-186">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-186">eq</span></span> |
| <span data-ttu-id="710a7-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="710a7-187">originalRequestId</span></span> | <span data-ttu-id="710a7-188">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-188">eq</span></span> |
| <span data-ttu-id="710a7-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="710a7-189">tokenIssuerName</span></span> | <span data-ttu-id="710a7-190">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-190">eq</span></span> |
| <span data-ttu-id="710a7-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="710a7-191">tokenIssuerType</span></span> | <span data-ttu-id="710a7-192">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-192">eq</span></span> |
| <span data-ttu-id="710a7-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="710a7-193">resourceDisplayName</span></span> | <span data-ttu-id="710a7-194">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-194">eq</span></span> |
| <span data-ttu-id="710a7-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="710a7-195">resourceId</span></span> | <span data-ttu-id="710a7-196">eq</span><span class="sxs-lookup"><span data-stu-id="710a7-196">eq</span></span> |
| <span data-ttu-id="710a7-197">сервицепринЦипалид</span><span class="sxs-lookup"><span data-stu-id="710a7-197">servicePrincipalId</span></span> | <span data-ttu-id="710a7-198">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-198">eq, startswith</span></span> |
| <span data-ttu-id="710a7-199">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="710a7-199">servicePrincipalName</span></span> | <span data-ttu-id="710a7-200">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-200">eq, startswith</span></span> |
| <span data-ttu-id="710a7-201">userAgent</span><span class="sxs-lookup"><span data-stu-id="710a7-201">userAgent</span></span> | <span data-ttu-id="710a7-202">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-202">eq, startswith</span></span> |
| <span data-ttu-id="710a7-203">алтернатесигниннаме</span><span class="sxs-lookup"><span data-stu-id="710a7-203">alternateSignInName</span></span> | <span data-ttu-id="710a7-204">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="710a7-204">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="710a7-205">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="710a7-205">Request headers</span></span>

| <span data-ttu-id="710a7-206">Имя</span><span class="sxs-lookup"><span data-stu-id="710a7-206">Name</span></span>      |<span data-ttu-id="710a7-207">Описание</span><span class="sxs-lookup"><span data-stu-id="710a7-207">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="710a7-208">Authorization</span><span class="sxs-lookup"><span data-stu-id="710a7-208">Authorization</span></span> | <span data-ttu-id="710a7-209">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="710a7-209">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="710a7-210">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="710a7-210">Request body</span></span>

<span data-ttu-id="710a7-211">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="710a7-211">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="710a7-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="710a7-212">Response</span></span>

<span data-ttu-id="710a7-213">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="710a7-213">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="710a7-214">Примеры</span><span class="sxs-lookup"><span data-stu-id="710a7-214">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="710a7-215">Пример 1: пользователь подписывается с помощью MFA, который активируется политикой условного доступа.</span><span class="sxs-lookup"><span data-stu-id="710a7-215">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="710a7-216">Основной способ проверки подлинности — Фидо.</span><span class="sxs-lookup"><span data-stu-id="710a7-216">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="710a7-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="710a7-217">Request</span></span>

<span data-ttu-id="710a7-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="710a7-218">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="710a7-219">HTTP</span><span class="sxs-lookup"><span data-stu-id="710a7-219">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="710a7-220">C#</span><span class="sxs-lookup"><span data-stu-id="710a7-220">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="710a7-221">JavaScript</span><span class="sxs-lookup"><span data-stu-id="710a7-221">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="710a7-222">Objective-C</span><span class="sxs-lookup"><span data-stu-id="710a7-222">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="710a7-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="710a7-223">Response</span></span>

<span data-ttu-id="710a7-224">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="710a7-224">The following is an example of the response.</span></span>

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
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="710a7-225">Пример 2: пользователь входит только с основной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="710a7-225">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="710a7-226">Первичная проверка подлинности осуществляется с помощью облачного пароля.</span><span class="sxs-lookup"><span data-stu-id="710a7-226">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="710a7-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="710a7-227">Request</span></span>

<span data-ttu-id="710a7-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="710a7-228">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="710a7-229">HTTP</span><span class="sxs-lookup"><span data-stu-id="710a7-229">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="710a7-230">C#</span><span class="sxs-lookup"><span data-stu-id="710a7-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="710a7-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="710a7-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="710a7-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="710a7-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="710a7-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="710a7-233">Response</span></span>

<span data-ttu-id="710a7-234">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="710a7-234">The following is an example of the response.</span></span>

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
