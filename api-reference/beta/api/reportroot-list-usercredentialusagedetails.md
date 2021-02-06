---
title: Список userCredentialUsageDetails
description: Получите список объектов userCredentialUsageDetails для заданного клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: e64d98318bcf9b083005f79156bc425a3b0d0fbc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134493"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="9c525-103">Список userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="9c525-103">List userCredentialUsageDetails</span></span>

<span data-ttu-id="9c525-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c525-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c525-105">Получите список объектов [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) для заданного клиента.</span><span class="sxs-lookup"><span data-stu-id="9c525-105">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="9c525-106">Сведения включают сведения о пользователе, состояние сброса и причину сбоя.</span><span class="sxs-lookup"><span data-stu-id="9c525-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c525-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c525-107">Permissions</span></span>

<span data-ttu-id="9c525-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c525-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c525-110">Permission type</span></span>                        | <span data-ttu-id="9c525-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c525-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9c525-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c525-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c525-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c525-113">Reports.Read.All</span></span> |
| <span data-ttu-id="9c525-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c525-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c525-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c525-115">Not supported.</span></span> |
| <span data-ttu-id="9c525-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c525-116">Application</span></span>                            | <span data-ttu-id="9c525-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c525-117">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c525-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c525-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c525-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9c525-119">Optional query parameters</span></span>

<span data-ttu-id="9c525-120">Эта функция поддерживает необязательный параметр запроса OData **$filter.**</span><span class="sxs-lookup"><span data-stu-id="9c525-120">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="9c525-121">Вы можете **применить $filter** к одному или более из следующих свойств ресурса [userCredentialUsageDetails.](../resources/usercredentialusagedetails.md)</span><span class="sxs-lookup"><span data-stu-id="9c525-121">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="9c525-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c525-122">Properties</span></span> | <span data-ttu-id="9c525-123">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="9c525-123">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="9c525-124">feature</span><span class="sxs-lookup"><span data-stu-id="9c525-124">feature</span></span> | <span data-ttu-id="9c525-125">Фильтрация по нужным типам данных об использовании (регистрация и сброс).</span><span class="sxs-lookup"><span data-stu-id="9c525-125">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="9c525-126">Пример: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="9c525-126">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="9c525-127">Поддерживаемые операторы фильтров: `eq`</span><span class="sxs-lookup"><span data-stu-id="9c525-127">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="9c525-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9c525-128">userDisplayName</span></span> | <span data-ttu-id="9c525-129">Фильтрация по отображаемой имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="9c525-129">Filter by user display name.</span></span> <span data-ttu-id="9c525-130">Пример: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="9c525-130">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="9c525-131">Поддерживаемые операторы фильтра: `eq` и `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="9c525-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="9c525-132">Поддерживается безчувствительности к делу.</span><span class="sxs-lookup"><span data-stu-id="9c525-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="9c525-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c525-133">userPrincipalName</span></span>  | <span data-ttu-id="9c525-134">Фильтрация по имени основного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9c525-134">Filter by user principal name.</span></span> <span data-ttu-id="9c525-135">Пример: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="9c525-135">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="9c525-136">Поддерживаемые операторы фильтра: `eq` и `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="9c525-136">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="9c525-137">Поддерживается безчувствительности к делу.</span><span class="sxs-lookup"><span data-stu-id="9c525-137">Supports case insensitive.</span></span> |
| <span data-ttu-id="9c525-138">isSuccess</span><span class="sxs-lookup"><span data-stu-id="9c525-138">isSuccess</span></span> | <span data-ttu-id="9c525-139">Фильтрация по статусу действия.</span><span class="sxs-lookup"><span data-stu-id="9c525-139">Filter by status of the activity.</span></span> <span data-ttu-id="9c525-140">Пример: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="9c525-140">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="9c525-141">Поддерживаемые операторы фильтра: `eq` и `orderby` .</span><span class="sxs-lookup"><span data-stu-id="9c525-141">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="9c525-142">authMethod</span><span class="sxs-lookup"><span data-stu-id="9c525-142">authMethod</span></span>  | <span data-ttu-id="9c525-143">Фильтрация по методам проверки подлинности, используемым во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="9c525-143">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="9c525-144">Пример: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="9c525-144">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="9c525-145">Поддерживаемые операторы фильтра: `eq` .</span><span class="sxs-lookup"><span data-stu-id="9c525-145">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="9c525-146">failureReason</span><span class="sxs-lookup"><span data-stu-id="9c525-146">failureReason</span></span> | <span data-ttu-id="9c525-147">Фильтрация по причине сбоя (если действие не удалось).</span><span class="sxs-lookup"><span data-stu-id="9c525-147">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="9c525-148">Пример: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="9c525-148">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="9c525-149">Поддерживаемые операторы фильтра: `eq` и `startswith()` .</span><span class="sxs-lookup"><span data-stu-id="9c525-149">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="9c525-150">Поддерживается безчувствительности к делу.</span><span class="sxs-lookup"><span data-stu-id="9c525-150">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="9c525-151">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c525-151">Request headers</span></span>

| <span data-ttu-id="9c525-152">Имя</span><span class="sxs-lookup"><span data-stu-id="9c525-152">Name</span></span>      |<span data-ttu-id="9c525-153">Описание</span><span class="sxs-lookup"><span data-stu-id="9c525-153">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c525-154">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c525-154">Authorization</span></span> | <span data-ttu-id="9c525-155">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9c525-155">Bearer {token}</span></span> |
| <span data-ttu-id="9c525-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9c525-156">Content-Type</span></span> | <span data-ttu-id="9c525-157">application/json</span><span class="sxs-lookup"><span data-stu-id="9c525-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c525-158">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c525-158">Request body</span></span>

<span data-ttu-id="9c525-159">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c525-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c525-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c525-160">Response</span></span>

<span data-ttu-id="9c525-161">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c525-161">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c525-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="9c525-162">Examples</span></span>

<span data-ttu-id="9c525-163">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9c525-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9c525-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c525-164">Request</span></span>

<span data-ttu-id="9c525-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c525-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c525-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c525-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[<span data-ttu-id="9c525-167">C#</span><span class="sxs-lookup"><span data-stu-id="9c525-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c525-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c525-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c525-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c525-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c525-170">Java</span><span class="sxs-lookup"><span data-stu-id="9c525-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9c525-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c525-171">Response</span></span>

<span data-ttu-id="9c525-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c525-172">The following is an example of the response.</span></span>

> <span data-ttu-id="9c525-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9c525-173">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9c525-174">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9c525-174">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 258

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


