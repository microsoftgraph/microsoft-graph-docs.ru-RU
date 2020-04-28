---
title: Список Усеркредентиалусажедетаилс
description: Получение списка объектов Усеркредентиалусажедетаилс для определенного клиента.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: df98f62df4465c43dede5f6cd293145b6c644e94
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386558"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="1048e-103">Список Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="1048e-103">List userCredentialUsageDetails</span></span>

<span data-ttu-id="1048e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1048e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1048e-105">Получение списка объектов [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="1048e-105">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="1048e-106">Сведения включают сведения о пользователе, состояние сброса и причину сбоя.</span><span class="sxs-lookup"><span data-stu-id="1048e-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="1048e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1048e-107">Permissions</span></span>

<span data-ttu-id="1048e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1048e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1048e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1048e-110">Permission type</span></span>                        | <span data-ttu-id="1048e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1048e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1048e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1048e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1048e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1048e-113">Reports.Read.All</span></span> |
| <span data-ttu-id="1048e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1048e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1048e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1048e-115">Not supported.</span></span> |
| <span data-ttu-id="1048e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1048e-116">Application</span></span>                            | <span data-ttu-id="1048e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1048e-117">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1048e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1048e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1048e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1048e-119">Optional query parameters</span></span>

<span data-ttu-id="1048e-120">Эта функция поддерживает необязательный параметр запроса OData **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="1048e-120">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="1048e-121">**$Filter** можно применить к одному или нескольким из следующих свойств ресурса [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="1048e-121">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="1048e-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="1048e-122">Properties</span></span> | <span data-ttu-id="1048e-123">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="1048e-123">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="1048e-124">состав</span><span class="sxs-lookup"><span data-stu-id="1048e-124">feature</span></span> | <span data-ttu-id="1048e-125">Фильтрация по типу требуемых данных (регистрация VS Reset).</span><span class="sxs-lookup"><span data-stu-id="1048e-125">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="1048e-126">Пример: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="1048e-126">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="1048e-127">Поддерживаемые операторы фильтра:`eq`</span><span class="sxs-lookup"><span data-stu-id="1048e-127">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="1048e-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1048e-128">userDisplayName</span></span> | <span data-ttu-id="1048e-129">Фильтрация по отображаемому имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="1048e-129">Filter by user display name.</span></span> <span data-ttu-id="1048e-130">Пример: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="1048e-130">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="1048e-131">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="1048e-131">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="1048e-132">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="1048e-132">Supports case insensitive.</span></span> |
| <span data-ttu-id="1048e-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1048e-133">userPrincipalName</span></span>  | <span data-ttu-id="1048e-134">Фильтрация по имени участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="1048e-134">Filter by user principal name.</span></span> <span data-ttu-id="1048e-135">Пример: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="1048e-135">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="1048e-136">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="1048e-136">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="1048e-137">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="1048e-137">Supports case insensitive.</span></span> |
| <span data-ttu-id="1048e-138">Выполнение</span><span class="sxs-lookup"><span data-stu-id="1048e-138">isSuccess</span></span> | <span data-ttu-id="1048e-139">Фильтрация по состоянию действия.</span><span class="sxs-lookup"><span data-stu-id="1048e-139">Filter by status of the activity.</span></span> <span data-ttu-id="1048e-140">Пример: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="1048e-140">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="1048e-141">Поддерживаемые операторы фильтра: `eq` и `orderby`.</span><span class="sxs-lookup"><span data-stu-id="1048e-141">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="1048e-142">аусмесод</span><span class="sxs-lookup"><span data-stu-id="1048e-142">authMethod</span></span>  | <span data-ttu-id="1048e-143">Фильтрация по методам проверки подлинности, используемым во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="1048e-143">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="1048e-144">Пример: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="1048e-144">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="1048e-145">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="1048e-145">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="1048e-146">failureReason</span><span class="sxs-lookup"><span data-stu-id="1048e-146">failureReason</span></span> | <span data-ttu-id="1048e-147">Фильтрация по причине сбоя (если действие завершилось с ошибкой).</span><span class="sxs-lookup"><span data-stu-id="1048e-147">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="1048e-148">Пример: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="1048e-148">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="1048e-149">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="1048e-149">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="1048e-150">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="1048e-150">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="1048e-151">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1048e-151">Request headers</span></span>

| <span data-ttu-id="1048e-152">Имя</span><span class="sxs-lookup"><span data-stu-id="1048e-152">Name</span></span>      |<span data-ttu-id="1048e-153">Описание</span><span class="sxs-lookup"><span data-stu-id="1048e-153">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1048e-154">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1048e-154">Authorization</span></span> | <span data-ttu-id="1048e-155">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1048e-155">Bearer {token}</span></span> |
| <span data-ttu-id="1048e-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1048e-156">Content-Type</span></span> | <span data-ttu-id="1048e-157">application/json</span><span class="sxs-lookup"><span data-stu-id="1048e-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1048e-158">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1048e-158">Request body</span></span>

<span data-ttu-id="1048e-159">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1048e-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1048e-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="1048e-160">Response</span></span>

<span data-ttu-id="1048e-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1048e-161">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1048e-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="1048e-162">Examples</span></span>

<span data-ttu-id="1048e-163">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1048e-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1048e-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="1048e-164">Request</span></span>

<span data-ttu-id="1048e-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1048e-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1048e-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="1048e-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[<span data-ttu-id="1048e-167">C#</span><span class="sxs-lookup"><span data-stu-id="1048e-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1048e-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1048e-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1048e-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1048e-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1048e-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="1048e-170">Response</span></span>

<span data-ttu-id="1048e-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1048e-171">The following is an example of the response.</span></span>

> <span data-ttu-id="1048e-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1048e-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1048e-173">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1048e-173">All the properties are returned from an actual call.</span></span>

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
