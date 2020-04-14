---
title: Список Кредентиалусеррегистратиондетаилс
description: Получение списка объектов Кредентиалусеррегистратиондетаилс для определенного клиента.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 7f530832a3b256dacf094e59f1193b096e5782dc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455710"
---
# <a name="list-credentialuserregistrationdetails"></a><span data-ttu-id="ad24e-103">Список Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="ad24e-103">List credentialUserRegistrationDetails</span></span>

<span data-ttu-id="ad24e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad24e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad24e-105">Получение списка объектов [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="ad24e-105">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad24e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad24e-106">Permissions</span></span>

<span data-ttu-id="ad24e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad24e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad24e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad24e-109">Permission type</span></span>                        | <span data-ttu-id="ad24e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad24e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ad24e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad24e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad24e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad24e-112">Reports.Read.All</span></span> |
| <span data-ttu-id="ad24e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad24e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad24e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad24e-114">Not supported.</span></span> |
| <span data-ttu-id="ad24e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad24e-115">Application</span></span>                            | <span data-ttu-id="ad24e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad24e-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad24e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad24e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad24e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad24e-118">Optional query parameters</span></span>

<span data-ttu-id="ad24e-119">Эта функция поддерживает необязательный параметр запроса OData **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="ad24e-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="ad24e-120">**$Filter** можно применить к одному или нескольким из следующих свойств ресурса [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="ad24e-120">You can apply **$filter** on one or more of the following properties of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) resource.</span></span>

| <span data-ttu-id="ad24e-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad24e-121">Properties</span></span> | <span data-ttu-id="ad24e-122">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="ad24e-122">Description and example</span></span> |
| --------- | ----------------------- |
| <span data-ttu-id="ad24e-123">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ad24e-123">userDisplayName</span></span> | <span data-ttu-id="ad24e-124">Фильтрация по имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="ad24e-124">Filter by user name.</span></span> <span data-ttu-id="ad24e-125">Пример: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-125">For example: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="ad24e-126">Поддерживаемые операторы фильтра: `eq`и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-126">Supported filter operators: `eq`, and `startswith()`.</span></span> <span data-ttu-id="ad24e-127">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="ad24e-127">Supports case insensitive.</span></span> |
| <span data-ttu-id="ad24e-128">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ad24e-128">userPrincipalName</span></span> | <span data-ttu-id="ad24e-129">Фильтрация по имени участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="ad24e-129">Filter by user principal name.</span></span> <span data-ttu-id="ad24e-130">Пример: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-130">For example: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span> <span data-ttu-id="ad24e-131">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="ad24e-132">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="ad24e-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="ad24e-133">аусмесодс</span><span class="sxs-lookup"><span data-stu-id="ad24e-133">authMethods</span></span> | <span data-ttu-id="ad24e-134">Фильтрация по методам проверки подлинности, используемым во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="ad24e-134">Filter by the authentication methods used during registration.</span></span> <span data-ttu-id="ad24e-135">Пример: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-135">For example: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`.</span></span> <span data-ttu-id="ad24e-136">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-136">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="ad24e-137">Регистрация</span><span class="sxs-lookup"><span data-stu-id="ad24e-137">isRegistered</span></span> | <span data-ttu-id="ad24e-138">Фильтр для пользователей, зарегистрированных для самостоятельного сброса пароля (SSPR).</span><span class="sxs-lookup"><span data-stu-id="ad24e-138">Filter for users who have registered for self-service password reset (SSPR).</span></span> <span data-ttu-id="ad24e-139">Пример: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-139">For example: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`.</span></span> <span data-ttu-id="ad24e-140">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-140">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="ad24e-141">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ad24e-141">isEnabled</span></span> | <span data-ttu-id="ad24e-142">Фильтрация для пользователей, которым был разрешен доступ к SSPR.</span><span class="sxs-lookup"><span data-stu-id="ad24e-142">Filter for users who have been enabled for SSPR.</span></span> <span data-ttu-id="ad24e-143">Пример: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-143">For example: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`.</span></span> <span data-ttu-id="ad24e-144">Поддерживаемые операторы филттер: `eq`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-144">Supported filtter operators: `eq`.</span></span> |
| <span data-ttu-id="ad24e-145">Поддержка</span><span class="sxs-lookup"><span data-stu-id="ad24e-145">isCapable</span></span> | <span data-ttu-id="ad24e-146">Фильтрация для пользователей, которые готовы к выполнению сброса пароля или многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="ad24e-146">Filter for users who are ready to perform password reset or multi-factor authentication (MFA).</span></span> <span data-ttu-id="ad24e-147">Пример: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-147">For example: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`.</span></span> <span data-ttu-id="ad24e-148">Поддерживаемые операторы фильтра:`eq`</span><span class="sxs-lookup"><span data-stu-id="ad24e-148">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="ad24e-149">исмфарегистеред</span><span class="sxs-lookup"><span data-stu-id="ad24e-149">isMfaRegistered</span></span> | <span data-ttu-id="ad24e-150">Фильтрация для пользователей, зарегистрированных для MFA.</span><span class="sxs-lookup"><span data-stu-id="ad24e-150">Filter for users who are registered for MFA.</span></span> <span data-ttu-id="ad24e-151">Пример: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-151">For example: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`.</span></span> <span data-ttu-id="ad24e-152">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="ad24e-152">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ad24e-153">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad24e-153">Request headers</span></span>

| <span data-ttu-id="ad24e-154">Имя</span><span class="sxs-lookup"><span data-stu-id="ad24e-154">Name</span></span>      |<span data-ttu-id="ad24e-155">Описание</span><span class="sxs-lookup"><span data-stu-id="ad24e-155">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad24e-156">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad24e-156">Authorization</span></span> | <span data-ttu-id="ad24e-157">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ad24e-157">Bearer {token}</span></span> |
| <span data-ttu-id="ad24e-158">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad24e-158">Content-Type</span></span> | <span data-ttu-id="ad24e-159">application/json</span><span class="sxs-lookup"><span data-stu-id="ad24e-159">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad24e-160">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad24e-160">Request body</span></span>

<span data-ttu-id="ad24e-161">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad24e-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad24e-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad24e-162">Response</span></span>

<span data-ttu-id="ad24e-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad24e-163">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad24e-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="ad24e-164">Examples</span></span>

<span data-ttu-id="ad24e-165">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ad24e-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ad24e-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad24e-166">Request</span></span>

<span data-ttu-id="ad24e-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad24e-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad24e-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad24e-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[<span data-ttu-id="ad24e-169">C#</span><span class="sxs-lookup"><span data-stu-id="ad24e-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad24e-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad24e-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad24e-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad24e-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad24e-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad24e-172">Response</span></span>

<span data-ttu-id="ad24e-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ad24e-173">The following is an example of the response.</span></span>

> <span data-ttu-id="ad24e-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad24e-174">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ad24e-175">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ad24e-175">All the properties are returned from an actual call.</span></span>

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
