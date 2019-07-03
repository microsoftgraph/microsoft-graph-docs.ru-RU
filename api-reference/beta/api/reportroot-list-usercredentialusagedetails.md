---
title: Список Усеркредентиалусажедетаилс
description: Получение списка объектов Усеркредентиалусажедетаилс для определенного клиента.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 813e5c538e7346973fd5cccf4d2751fefc1fdd48
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465001"
---
# <a name="list-usercredentialusagedetails"></a><span data-ttu-id="42344-103">Список Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="42344-103">List userCredentialUsageDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42344-104">Получение списка объектов [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="42344-104">Get a list of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects for a given tenant.</span></span> <span data-ttu-id="42344-105">Сведения включают сведения о пользователе, состояние сброса и причину сбоя.</span><span class="sxs-lookup"><span data-stu-id="42344-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="permissions"></a><span data-ttu-id="42344-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42344-106">Permissions</span></span>

<span data-ttu-id="42344-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42344-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42344-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42344-109">Permission type</span></span>                        | <span data-ttu-id="42344-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42344-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="42344-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42344-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42344-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="42344-112">Reports.Read.All</span></span> |
| <span data-ttu-id="42344-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42344-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42344-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42344-114">Not supported.</span></span> |
| <span data-ttu-id="42344-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42344-115">Application</span></span>                            | <span data-ttu-id="42344-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="42344-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42344-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42344-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42344-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42344-118">Optional query parameters</span></span>

<span data-ttu-id="42344-119">Эта функция поддерживает необязательный параметр запроса OData **$Filter**.</span><span class="sxs-lookup"><span data-stu-id="42344-119">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="42344-120">**$Filter** можно применить к одному или нескольким из следующих свойств ресурса [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) .</span><span class="sxs-lookup"><span data-stu-id="42344-120">You can apply **$filter** on one or more of the following properties of the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) resource.</span></span>

| <span data-ttu-id="42344-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="42344-121">Properties</span></span> | <span data-ttu-id="42344-122">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="42344-122">Description and example</span></span> |
|:--------- |:----------- |
| <span data-ttu-id="42344-123">состав</span><span class="sxs-lookup"><span data-stu-id="42344-123">feature</span></span> | <span data-ttu-id="42344-124">Фильтрация по типу требуемых данных (регистрация VS Reset).</span><span class="sxs-lookup"><span data-stu-id="42344-124">Filter by type of usage data that you want (registration vs reset).</span></span> <span data-ttu-id="42344-125">Пример: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="42344-125">For example: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="42344-126">Поддерживаемые операторы фильтра:`eq`</span><span class="sxs-lookup"><span data-stu-id="42344-126">Supported filter operators: `eq`</span></span> |
| <span data-ttu-id="42344-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="42344-127">userDisplayName</span></span> | <span data-ttu-id="42344-128">Фильтрация по отображаемому имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="42344-128">Filter by user display name.</span></span> <span data-ttu-id="42344-129">Пример: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="42344-129">For example: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`.</span></span> <span data-ttu-id="42344-130">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="42344-130">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="42344-131">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="42344-131">Supports case insensitive.</span></span> |
| <span data-ttu-id="42344-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42344-132">userPrincipalName</span></span>  | <span data-ttu-id="42344-133">Фильтрация по имени участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="42344-133">Filter by user principal name.</span></span> <span data-ttu-id="42344-134">Пример: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="42344-134">For example: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.</span></span>    <span data-ttu-id="42344-135">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="42344-135">Supported filter  operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="42344-136">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="42344-136">Supports case insensitive.</span></span> |
| <span data-ttu-id="42344-137">Выполнение</span><span class="sxs-lookup"><span data-stu-id="42344-137">isSuccess</span></span> | <span data-ttu-id="42344-138">Фильтрация по состоянию действия.</span><span class="sxs-lookup"><span data-stu-id="42344-138">Filter by status of the activity.</span></span> <span data-ttu-id="42344-139">Пример: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span><span class="sxs-lookup"><span data-stu-id="42344-139">For example: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`.</span></span> <span data-ttu-id="42344-140">Поддерживаемые операторы фильтра: `eq` и `orderby`.</span><span class="sxs-lookup"><span data-stu-id="42344-140">Supported filter operators: `eq` and `orderby`.</span></span> |
| <span data-ttu-id="42344-141">Аусмесод</span><span class="sxs-lookup"><span data-stu-id="42344-141">authMethod</span></span>  | <span data-ttu-id="42344-142">Фильтрация по методам проверки подлинности, используемым во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="42344-142">Filter by the authentication methods using during registration.</span></span> <span data-ttu-id="42344-143">Пример: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span><span class="sxs-lookup"><span data-stu-id="42344-143">For example: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`.</span></span> <span data-ttu-id="42344-144">Поддерживаемые операторы фильтра: `eq`.</span><span class="sxs-lookup"><span data-stu-id="42344-144">Supported filter operators: `eq`.</span></span> |
| <span data-ttu-id="42344-145">failureReason</span><span class="sxs-lookup"><span data-stu-id="42344-145">failureReason</span></span> | <span data-ttu-id="42344-146">Фильтрация по причине сбоя (если действие завершилось с ошибкой).</span><span class="sxs-lookup"><span data-stu-id="42344-146">Filter by failure reason (if the activity has failed).</span></span> <span data-ttu-id="42344-147">Пример: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span><span class="sxs-lookup"><span data-stu-id="42344-147">For example: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`.</span></span> <span data-ttu-id="42344-148">Поддерживаемые операторы фильтра: `eq` и `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="42344-148">Supported filter operators: `eq` and `startswith()`.</span></span> <span data-ttu-id="42344-149">Поддерживает не зависящий от регистра.</span><span class="sxs-lookup"><span data-stu-id="42344-149">Supports case insensitive.</span></span> |


## <a name="request-headers"></a><span data-ttu-id="42344-150">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42344-150">Request headers</span></span>

| <span data-ttu-id="42344-151">Имя</span><span class="sxs-lookup"><span data-stu-id="42344-151">Name</span></span>      |<span data-ttu-id="42344-152">Описание</span><span class="sxs-lookup"><span data-stu-id="42344-152">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42344-153">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42344-153">Authorization</span></span> | <span data-ttu-id="42344-154">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="42344-154">Bearer {token}</span></span> |
| <span data-ttu-id="42344-155">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42344-155">Content-Type</span></span> | <span data-ttu-id="42344-156">application/json</span><span class="sxs-lookup"><span data-stu-id="42344-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="42344-157">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42344-157">Request body</span></span>

<span data-ttu-id="42344-158">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42344-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42344-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="42344-159">Response</span></span>

<span data-ttu-id="42344-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усеркредентиалусажедетаилс](../resources/usercredentialusagedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42344-160">If successful, this method returns a `200 OK` response code and a collection of [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42344-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="42344-161">Examples</span></span>

<span data-ttu-id="42344-162">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="42344-162">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="42344-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="42344-163">Request</span></span>

<span data-ttu-id="42344-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42344-164">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```

### <a name="response"></a><span data-ttu-id="42344-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="42344-165">Response</span></span>

<span data-ttu-id="42344-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="42344-166">The following is an example of the response.</span></span>

> <span data-ttu-id="42344-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="42344-167">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="42344-168">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="42344-168">All the properties are returned from an actual call.</span></span>

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