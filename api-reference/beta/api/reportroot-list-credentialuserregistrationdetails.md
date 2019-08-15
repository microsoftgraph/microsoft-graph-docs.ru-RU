---
title: Список Кредентиалусеррегистратиондетаилс
description: Получение списка объектов Кредентиалусеррегистратиондетаилс для определенного клиента.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: e11e05c01ec84eda9ef4711e398c810fccfcdf36
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410960"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="c6f28-103">Список Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="c6f28-103">List credentialUserRegistrationDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6f28-104">Получение списка объектов [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="c6f28-104">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6f28-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6f28-105">Permissions</span></span>

<span data-ttu-id="c6f28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6f28-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6f28-108">Permission type</span></span>                        | <span data-ttu-id="c6f28-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6f28-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c6f28-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6f28-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6f28-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6f28-111">Reports.Read.All</span></span> |
| <span data-ttu-id="c6f28-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6f28-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6f28-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6f28-113">Not supported.</span></span> |
| <span data-ttu-id="c6f28-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6f28-114">Application</span></span>                            | <span data-ttu-id="c6f28-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6f28-115">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6f28-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6f28-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6f28-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c6f28-117">Optional query parameters</span></span>

<span data-ttu-id="c6f28-118">Эта функция поддерживает необязательный параметр запроса OData **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="c6f28-118">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="c6f28-119">**$Filter** можно применить к одному или нескольким из следующих свойств ресурса [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="c6f28-119">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="c6f28-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6f28-120">Properties</span></span> | <span data-ttu-id="c6f28-121">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="c6f28-121">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="c6f28-122">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c6f28-122">userDisplayName</span></span> | <span data-ttu-id="c6f28-123">Фильтрация по имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6f28-123">Filter by user name.</span></span> <span data-ttu-id="c6f28-124">Пример: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-124">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="c6f28-125">Поддерживаемые операторы фильтра: `eq`и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-125">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="c6f28-126">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="c6f28-126">Supports case insensitive.</span></span> |
| <span data-ttu-id="c6f28-127">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c6f28-127">userPrincipalName</span></span> | <span data-ttu-id="c6f28-128">Фильтрация по имени участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6f28-128">Filter by user principal name.</span></span> <span data-ttu-id="c6f28-129">Пример: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-129">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="c6f28-130">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="c6f28-131">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="c6f28-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="c6f28-132">аусмесодс</span><span class="sxs-lookup"><span data-stu-id="c6f28-132">authMethods</span></span> | <span data-ttu-id="c6f28-133">Фильтрация по методам проверки подлинности, используемым во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="c6f28-133">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="c6f28-134">Пример: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-134">For example: `/reports/userCredentialUsageDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="c6f28-135">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-135">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="c6f28-136">Регистрация</span><span class="sxs-lookup"><span data-stu-id="c6f28-136">isRegistered</span></span> | <span data-ttu-id="c6f28-137">Фильтр для пользователей, зарегистрированных для самостоятельного сброса пароля (SSPR).</span><span class="sxs-lookup"><span data-stu-id="c6f28-137">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="c6f28-138">Пример: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-138">For example: `/reports/userCredentialUsageDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="c6f28-139">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-139">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="c6f28-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c6f28-140">isEnabled</span></span> | <span data-ttu-id="c6f28-141">Фильтрация для пользователей, которым был разрешен доступ к SSPR.</span><span class="sxs-lookup"><span data-stu-id="c6f28-141">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="c6f28-142">Пример: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-142">For example: `/reports/userCredentialUsageDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="c6f28-143">Поддерживаемые операторы филттер: `eq`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-143">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="c6f28-144">Поддержка</span><span class="sxs-lookup"><span data-stu-id="c6f28-144">isCapable</span></span> | <span data-ttu-id="c6f28-145">Фильтрация для пользователей, которые готовы к выполнению сброса пароля или многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="c6f28-145">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="c6f28-146">Пример: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-146">For example: `/reports/userCredentialUsageDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="c6f28-147">Поддерживаемые операторы фильтра:`eq`</span><span class="sxs-lookup"><span data-stu-id="c6f28-147">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="c6f28-148">исмфарегистеред</span><span class="sxs-lookup"><span data-stu-id="c6f28-148">isMfaRegistered</span></span> | <span data-ttu-id="c6f28-149">Фильтрация для пользователей, зарегистрированных для MFA.</span><span class="sxs-lookup"><span data-stu-id="c6f28-149">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="c6f28-150">Пример: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-150">For example: `/reports/userCredentialUsageDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="c6f28-151">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="c6f28-151">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c6f28-152">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6f28-152">Request headers</span></span>

| <span data-ttu-id="c6f28-153">Имя</span><span class="sxs-lookup"><span data-stu-id="c6f28-153">Name</span></span>      |<span data-ttu-id="c6f28-154">Описание</span><span class="sxs-lookup"><span data-stu-id="c6f28-154">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6f28-155">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6f28-155">Authorization</span></span> | <span data-ttu-id="c6f28-156">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c6f28-156">Bearer {token}</span></span> |
| <span data-ttu-id="c6f28-157">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6f28-157">Content-Type</span></span> | <span data-ttu-id="c6f28-158">application/json</span><span class="sxs-lookup"><span data-stu-id="c6f28-158">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6f28-159">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6f28-159">Request body</span></span>

<span data-ttu-id="c6f28-160">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6f28-160">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6f28-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6f28-161">Response</span></span>

<span data-ttu-id="c6f28-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6f28-162">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6f28-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="c6f28-163">Examples</span></span>

<span data-ttu-id="c6f28-164">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c6f28-164">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c6f28-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6f28-165">Request</span></span>

<span data-ttu-id="c6f28-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6f28-166">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c6f28-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6f28-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c6f28-168">C#</span><span class="sxs-lookup"><span data-stu-id="c6f28-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6f28-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6f28-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c6f28-170">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c6f28-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c6f28-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6f28-171">Response</span></span>

<span data-ttu-id="c6f28-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c6f28-172">The following is an example of the response.</span></span>

> <span data-ttu-id="c6f28-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c6f28-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c6f28-174">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c6f28-174">All the properties are returned from an actual call.</span></span>

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
