---
title: Перечисление входов
doc_type: apiPageType
description: Получение списка входов пользователей в клиенте Azure Active Directory.
localization_priority: Normal
author: kholtz
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cf580035957a5605fdd013a1d045548fcae4f94f
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123002"
---
# <a name="list-signins"></a><span data-ttu-id="51b82-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="51b82-103">List signIns</span></span>

<span data-ttu-id="51b82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51b82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b82-105">Получение списка объектов [SignIn](../resources/signin.md) .</span><span class="sxs-lookup"><span data-stu-id="51b82-105">Get a list of [signIn](../resources/signin.md) objects.</span></span> <span data-ttu-id="51b82-106">В этом списке содержатся входы пользователей для клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="51b82-106">The list contains the user sign-ins for your Azure Active Directory tenant.</span></span> <span data-ttu-id="51b82-107">Входы, в которых имя пользователя и пароль передаются в составе маркера авторизации, а успешные Федеративные входы в систему в данный момент включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="51b82-107">Sign-ins where a username and password are passed as part of authorization token, and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="51b82-108">Первыми возвращаются последние входные.</span><span class="sxs-lookup"><span data-stu-id="51b82-108">The most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="51b82-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51b82-109">Permissions</span></span>

<span data-ttu-id="51b82-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51b82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51b82-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51b82-112">Permission type</span></span> | <span data-ttu-id="51b82-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51b82-113">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="51b82-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51b82-114">Delegated (work or school account)</span></span> | <span data-ttu-id="51b82-115">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="51b82-115">AuditLog.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="51b82-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51b82-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51b82-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="51b82-117">Not supported</span></span> |
| <span data-ttu-id="51b82-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51b82-118">Application</span></span> | <span data-ttu-id="51b82-119">Аудитлог. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="51b82-119">AuditLog.Read.All, Directory.Read.All</span></span> | 

<span data-ttu-id="51b82-120">Кроме того, приложения должны быть должным образом зарегистрированы в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="51b82-120">In addition, apps must be properly registered to Azure Active Directory.</span></span>

## <a name="http-request"></a><span data-ttu-id="51b82-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51b82-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51b82-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51b82-122">Optional query parameters</span></span>

<span data-ttu-id="51b82-123">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="51b82-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="51b82-124">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="51b82-124">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

| <span data-ttu-id="51b82-125">Имя</span><span class="sxs-lookup"><span data-stu-id="51b82-125">Name</span></span> | <span data-ttu-id="51b82-126">Описание</span><span class="sxs-lookup"><span data-stu-id="51b82-126">Description</span></span> | <span data-ttu-id="51b82-127">Пример</span><span class="sxs-lookup"><span data-stu-id="51b82-127">Example</span></span> |
|:---- |:----------- |:------- |
| [<span data-ttu-id="51b82-128">$filter</span><span class="sxs-lookup"><span data-stu-id="51b82-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)| <span data-ttu-id="51b82-129">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="51b82-129">Filters results (rows).</span></span> | `/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24` |
| [<span data-ttu-id="51b82-130">$top</span><span class="sxs-lookup"><span data-stu-id="51b82-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter) | <span data-ttu-id="51b82-131">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="51b82-131">Sets the page size of results.</span></span> | `/auditLogs/signIns?$top=1` |
| [<span data-ttu-id="51b82-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="51b82-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter) | <span data-ttu-id="51b82-133">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="51b82-133">Retrieves the next page of results from result sets that span multiple pages.</span></span> |`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="51b82-134">Атрибуты, поддерживаемые параметром $filter</span><span class="sxs-lookup"><span data-stu-id="51b82-134">Attributes supported by $filter parameter</span></span>

| <span data-ttu-id="51b82-135">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="51b82-135">Attribute Name</span></span> | <span data-ttu-id="51b82-136">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="51b82-136">Supported operators</span></span> |
|:-------------- |:------------------- |
| <span data-ttu-id="51b82-137">id</span><span class="sxs-lookup"><span data-stu-id="51b82-137">id</span></span> | <span data-ttu-id="51b82-138">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-138">eq</span></span> |
| <span data-ttu-id="51b82-139">userId</span><span class="sxs-lookup"><span data-stu-id="51b82-139">userId</span></span> | <span data-ttu-id="51b82-140">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-140">eq</span></span> |
| <span data-ttu-id="51b82-141">appId</span><span class="sxs-lookup"><span data-stu-id="51b82-141">appId</span></span> | <span data-ttu-id="51b82-142">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-142">eq</span></span> |
| <span data-ttu-id="51b82-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51b82-143">createdDateTime</span></span> | <span data-ttu-id="51b82-144">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="51b82-144">eq, le, ge</span></span> |
| <span data-ttu-id="51b82-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="51b82-145">userDisplayName</span></span> | <span data-ttu-id="51b82-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-146">eq, startswith</span></span> |
| <span data-ttu-id="51b82-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51b82-147">userPrincipalName</span></span> | <span data-ttu-id="51b82-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-148">eq, startswith</span></span> |
| <span data-ttu-id="51b82-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="51b82-149">appDisplayName</span></span> | <span data-ttu-id="51b82-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-150">eq, startswith</span></span> |
| <span data-ttu-id="51b82-151">аусентикатионрекуиремент</span><span class="sxs-lookup"><span data-stu-id="51b82-151">authenticationRequirement</span></span> |<span data-ttu-id="51b82-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-152">eq, startswith</span></span> |
| <span data-ttu-id="51b82-153">ipAddress</span><span class="sxs-lookup"><span data-stu-id="51b82-153">ipAddress</span></span> | <span data-ttu-id="51b82-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-154">eq, startswith</span></span> |
| <span data-ttu-id="51b82-155">location/city</span><span class="sxs-lookup"><span data-stu-id="51b82-155">location/city</span></span> | <span data-ttu-id="51b82-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-156">eq, startswith</span></span> |
| <span data-ttu-id="51b82-157">location/state</span><span class="sxs-lookup"><span data-stu-id="51b82-157">location/state</span></span> | <span data-ttu-id="51b82-158">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-158">eq, startswith</span></span> |
| <span data-ttu-id="51b82-159">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="51b82-159">location/countryOrRegion</span></span> | <span data-ttu-id="51b82-160">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-160">eq, startswith</span></span> |
| <span data-ttu-id="51b82-161">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="51b82-161">status/errorCode</span></span> | <span data-ttu-id="51b82-162">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-162">eq</span></span> |
| <span data-ttu-id="51b82-163">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="51b82-163">initiatedBy/user/id</span></span> | <span data-ttu-id="51b82-164">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-164">eq</span></span> |
| <span data-ttu-id="51b82-165">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="51b82-165">initiatedBy/user/displayName</span></span> | <span data-ttu-id="51b82-166">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-166">eq</span></span> |
| <span data-ttu-id="51b82-167">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51b82-167">initiatedBy/user/userPrincipalName</span></span> | <span data-ttu-id="51b82-168">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-168">eq, startswith</span></span> |
| <span data-ttu-id="51b82-169">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="51b82-169">clientAppUsed</span></span> | <span data-ttu-id="51b82-170">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-170">eq</span></span> |
| <span data-ttu-id="51b82-171">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="51b82-171">conditionalAccessStatus</span></span> | <span data-ttu-id="51b82-172">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-172">eq</span></span> |
| <span data-ttu-id="51b82-173">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="51b82-173">deviceDetail/browser</span></span> | <span data-ttu-id="51b82-174">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-174">eq, startswith</span></span> |
| <span data-ttu-id="51b82-175">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="51b82-175">deviceDetail/operatingSystem</span></span> | <span data-ttu-id="51b82-176">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-176">eq, startswith</span></span> |
| <span data-ttu-id="51b82-177">correlationId</span><span class="sxs-lookup"><span data-stu-id="51b82-177">correlationId</span></span> | <span data-ttu-id="51b82-178">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-178">eq</span></span> |
| <span data-ttu-id="51b82-179">riskDetail</span><span class="sxs-lookup"><span data-stu-id="51b82-179">riskDetail</span></span> | <span data-ttu-id="51b82-180">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-180">eq</span></span> |
| <span data-ttu-id="51b82-181">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="51b82-181">riskLevelAggregated</span></span> | <span data-ttu-id="51b82-182">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-182">eq</span></span> |
| <span data-ttu-id="51b82-183">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="51b82-183">riskLevelDuringSignIn</span></span> | <span data-ttu-id="51b82-184">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-184">eq</span></span> |
| <span data-ttu-id="51b82-185">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="51b82-185">riskEventTypes</span></span> | <span data-ttu-id="51b82-186">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-186">eq</span></span> |
| <span data-ttu-id="51b82-187">riskEventTypes_v2</span><span class="sxs-lookup"><span data-stu-id="51b82-187">riskEventTypes_v2</span></span> | <span data-ttu-id="51b82-188">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-188">eq, startswith</span></span> |
| <span data-ttu-id="51b82-189">riskState</span><span class="sxs-lookup"><span data-stu-id="51b82-189">riskState</span></span> | <span data-ttu-id="51b82-190">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-190">eq</span></span> |
| <span data-ttu-id="51b82-191">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="51b82-191">originalRequestId</span></span> | <span data-ttu-id="51b82-192">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-192">eq</span></span> |
| <span data-ttu-id="51b82-193">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="51b82-193">tokenIssuerName</span></span> | <span data-ttu-id="51b82-194">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-194">eq</span></span> |
| <span data-ttu-id="51b82-195">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="51b82-195">tokenIssuerType</span></span> | <span data-ttu-id="51b82-196">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-196">eq</span></span> |
| <span data-ttu-id="51b82-197">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="51b82-197">resourceDisplayName</span></span> | <span data-ttu-id="51b82-198">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-198">eq</span></span> |
| <span data-ttu-id="51b82-199">resourceId</span><span class="sxs-lookup"><span data-stu-id="51b82-199">resourceId</span></span> | <span data-ttu-id="51b82-200">eq</span><span class="sxs-lookup"><span data-stu-id="51b82-200">eq</span></span> |
| <span data-ttu-id="51b82-201">сервицепринЦипалид</span><span class="sxs-lookup"><span data-stu-id="51b82-201">servicePrincipalId</span></span> | <span data-ttu-id="51b82-202">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-202">eq, startswith</span></span> |
| <span data-ttu-id="51b82-203">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="51b82-203">servicePrincipalName</span></span> | <span data-ttu-id="51b82-204">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-204">eq, startswith</span></span> |
| <span data-ttu-id="51b82-205">userAgent</span><span class="sxs-lookup"><span data-stu-id="51b82-205">userAgent</span></span> | <span data-ttu-id="51b82-206">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-206">eq, startswith</span></span> |
| <span data-ttu-id="51b82-207">алтернатесигниннаме</span><span class="sxs-lookup"><span data-stu-id="51b82-207">alternateSignInName</span></span> | <span data-ttu-id="51b82-208">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51b82-208">eq, startswith</span></span> |

## <a name="request-headers"></a><span data-ttu-id="51b82-209">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51b82-209">Request headers</span></span>

| <span data-ttu-id="51b82-210">Имя</span><span class="sxs-lookup"><span data-stu-id="51b82-210">Name</span></span>      |<span data-ttu-id="51b82-211">Описание</span><span class="sxs-lookup"><span data-stu-id="51b82-211">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51b82-212">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51b82-212">Authorization</span></span> | <span data-ttu-id="51b82-213">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="51b82-213">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="51b82-214">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51b82-214">Request body</span></span>

<span data-ttu-id="51b82-215">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51b82-215">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51b82-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="51b82-216">Response</span></span>

<span data-ttu-id="51b82-217">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51b82-217">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51b82-218">Примеры</span><span class="sxs-lookup"><span data-stu-id="51b82-218">Examples</span></span>

### <a name="example-1-user-signs-in-using-mfa-which-is-triggered-by-a-conditional-access-policy-primary-authentication-is-through-fido"></a><span data-ttu-id="51b82-219">Пример 1: пользователь подписывается с помощью MFA, который активируется политикой условного доступа.</span><span class="sxs-lookup"><span data-stu-id="51b82-219">Example 1: User signs in using MFA, which is triggered by a conditional access policy.</span></span> <span data-ttu-id="51b82-220">Основной способ проверки подлинности — Фидо.</span><span class="sxs-lookup"><span data-stu-id="51b82-220">Primary authentication is through FIDO.</span></span>

#### <a name="request"></a><span data-ttu-id="51b82-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="51b82-221">Request</span></span>

<span data-ttu-id="51b82-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51b82-222">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51b82-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="51b82-223">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="51b82-224">C#</span><span class="sxs-lookup"><span data-stu-id="51b82-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51b82-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51b82-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51b82-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51b82-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="51b82-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="51b82-227">Response</span></span>

<span data-ttu-id="51b82-228">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51b82-228">The following is an example of the response.</span></span>

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
            "id": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-1111-5555-b4e2-a37c6808512d",
            "appId": "de8bc8b5-5555-6666-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "authenticationRequirement": "multiFactorAuthentication",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Safari/537.36 Edg/80.0.361.66",
            "correlationId": "d79f5bee-blah-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "66ea54eb-blah-4ee5-be62-ff5a759b0100",
            "isInteractive": true,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 541,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "authenticationMethodsUsed": [],
            "alternateSignInName": "testaccount2.contoso.com",
            "servicePrincipalName": null,
            "servicePrincipalId": "",
            "mfaDetail": null,
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "",
                "displayName": null,
                "operatingSystem": "Windows 10",
                "browser": "Edge 80.0.361",
                "isCompliant": null,
                "isManaged": null,
                "trustType": null
            },
            "location": {
                "city": "Redmond",
                "state": "Washington",
                "countryOrRegion": "US",
                "geoCoordinates": {
                    "altitude": null,
                    "latitude": 47.68050003051758,
                    "longitude": -122.12094116210938
                }
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "de7e60eb-ed89-4d73-8205-2227def6b7c9",
                    "displayName": "SharePoint limited access for guest workers",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none"
                },
               
            ],
            "authenticationProcessingDetails": [],
            "networkLocationDetails": [],
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
            "authenticationRequirementPolicies": []
        }
    ]
}
```
### <a name="example-2-user-signs-in-with-only-primary-authentication-primary-authentication-is-through-cloud-password"></a><span data-ttu-id="51b82-229">Пример 2: пользователь входит только с основной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="51b82-229">Example 2: User signs in with only primary authentication.</span></span> <span data-ttu-id="51b82-230">Первичная проверка подлинности осуществляется с помощью облачного пароля.</span><span class="sxs-lookup"><span data-stu-id="51b82-230">Primary authentication is through cloud password.</span></span>

#### <a name="request"></a><span data-ttu-id="51b82-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="51b82-231">Request</span></span>

<span data-ttu-id="51b82-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51b82-232">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="51b82-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="51b82-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="51b82-234">C#</span><span class="sxs-lookup"><span data-stu-id="51b82-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51b82-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51b82-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51b82-236">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51b82-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51b82-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="51b82-237">Response</span></span>

<span data-ttu-id="51b82-238">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="51b82-238">The following is an example of the response.</span></span>

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
      "userPrincipalName":"jdoe@contoso.com",
      "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
       "authenticationRequirement": "singleFactorAuthentication",
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
