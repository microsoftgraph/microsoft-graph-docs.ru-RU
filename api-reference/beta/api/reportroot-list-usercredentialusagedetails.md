---
title: Список Усеркредентиалусажедетаилс
description: Получение списка объектов Усеркредентиалусажедетаилс для определенного клиента.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 39ff2172ecaaa7f51c16961aef1630e0ddb0e70c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724808"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="51651-103">Список Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="51651-103">List userCredentialUsageDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51651-104">Получение списка объектов [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="51651-104">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="51651-105">Сведения включают сведения о пользователе, состояние сброса и причину сбоя.</span><span class="sxs-lookup"><span data-stu-id="51651-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="51651-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51651-106">Permissions</span></span>

<span data-ttu-id="51651-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51651-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51651-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51651-109">Permission type</span></span>                        | <span data-ttu-id="51651-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51651-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51651-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51651-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="51651-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="51651-112">Reports.Read.All</span></span> |
| <span data-ttu-id="51651-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51651-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51651-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51651-114">Not supported.</span></span> |
| <span data-ttu-id="51651-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51651-115">Application</span></span>                            | <span data-ttu-id="51651-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="51651-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51651-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51651-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51651-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51651-118">Optional query parameters</span></span>

<span data-ttu-id="51651-119">Эта функция поддерживает необязательный параметр запроса OData **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="51651-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="51651-120">**$Filter** можно применить к одному или нескольким из следующих свойств ресурса [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="51651-120">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="51651-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="51651-121">Properties</span></span> | <span data-ttu-id="51651-122">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="51651-122">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="51651-123">состав</span><span class="sxs-lookup"><span data-stu-id="51651-123">feature</span></span> | <span data-ttu-id="51651-124">Фильтрация по типу требуемых данных (регистрация VS Reset).</span><span class="sxs-lookup"><span data-stu-id="51651-124">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="51651-125">Пример: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="51651-125">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="51651-126">Поддерживаемые операторы фильтра:`eq`</span><span class="sxs-lookup"><span data-stu-id="51651-126">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="51651-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="51651-127">userDisplayName</span></span> | <span data-ttu-id="51651-128">Фильтрация по отображаемому имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="51651-128">Filter by user display name.</span></span> <span data-ttu-id="51651-129">Пример: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="51651-129">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="51651-130">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="51651-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="51651-131">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="51651-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="51651-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51651-132">userPrincipalName</span></span>  | <span data-ttu-id="51651-133">Фильтрация по имени участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="51651-133">Filter by user principal name.</span></span> <span data-ttu-id="51651-134">Пример: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="51651-134">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="51651-135">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="51651-135">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="51651-136">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="51651-136">Supports case insensitive.</span></span> |
| <span data-ttu-id="51651-137">Выполнение</span><span class="sxs-lookup"><span data-stu-id="51651-137">isSuccess</span></span> | <span data-ttu-id="51651-138">Фильтрация по состоянию действия.</span><span class="sxs-lookup"><span data-stu-id="51651-138">Filter by status of the activity.</span></span> <span data-ttu-id="51651-139">Пример: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="51651-139">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="51651-140">Поддерживаемые операторы фильтра: `eq` и `orderby`.</span><span class="sxs-lookup"><span data-stu-id="51651-140">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="51651-141">аусмесод</span><span class="sxs-lookup"><span data-stu-id="51651-141">authMethod</span></span>  | <span data-ttu-id="51651-142">Фильтрация по методам проверки подлинности, используемым во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="51651-142">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="51651-143">Пример: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="51651-143">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="51651-144">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="51651-144">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="51651-145">failureReason</span><span class="sxs-lookup"><span data-stu-id="51651-145">failureReason</span></span> | <span data-ttu-id="51651-146">Фильтрация по причине сбоя (если действие завершилось с ошибкой).</span><span class="sxs-lookup"><span data-stu-id="51651-146">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="51651-147">Пример: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="51651-147">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="51651-148">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="51651-148">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="51651-149">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="51651-149">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="51651-150">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51651-150">Request headers</span></span>

| <span data-ttu-id="51651-151">Имя</span><span class="sxs-lookup"><span data-stu-id="51651-151">Name</span></span>      |<span data-ttu-id="51651-152">Описание</span><span class="sxs-lookup"><span data-stu-id="51651-152">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51651-153">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51651-153">Authorization</span></span> | <span data-ttu-id="51651-154">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="51651-154">Bearer {token}</span></span> |
| <span data-ttu-id="51651-155">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51651-155">Content-Type</span></span> | <span data-ttu-id="51651-156">application/json</span><span class="sxs-lookup"><span data-stu-id="51651-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="51651-157">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51651-157">Request body</span></span>

<span data-ttu-id="51651-158">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51651-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51651-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="51651-159">Response</span></span>

<span data-ttu-id="51651-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51651-160">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51651-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="51651-161">Examples</span></span>

<span data-ttu-id="51651-162">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="51651-162">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="51651-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="51651-163">Request</span></span>

<span data-ttu-id="51651-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51651-164">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="51651-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="51651-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51651-166">C#</span><span class="sxs-lookup"><span data-stu-id="51651-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51651-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51651-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51651-168">Цель — C</span><span class="sxs-lookup"><span data-stu-id="51651-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51651-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="51651-169">Response</span></span>

<span data-ttu-id="51651-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="51651-170">The following is an example of the response.</span></span>

> <span data-ttu-id="51651-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="51651-171">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51651-172">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51651-172">All the properties are returned from an actual call.</span></span>

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
