---
title: 'reportRoot: getCredentialUsageSummary'
description: Report the current state of how many users in your organization are using self-service password reset capabilities.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 56015afd7bc5589d518277df555ac511b7f91657
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131357"
---
# <a name="reportroot-getcredentialusagesummary"></a><span data-ttu-id="e3280-103">reportRoot: getCredentialUsageSummary</span><span class="sxs-lookup"><span data-stu-id="e3280-103">reportRoot: getCredentialUsageSummary</span></span>

<span data-ttu-id="e3280-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3280-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3280-105">Report the current state of how many users in your organization used the self-service password reset capabilities.</span><span class="sxs-lookup"><span data-stu-id="e3280-105">Report the current state of how many users in your organization used the self-service password reset capabilities.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3280-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3280-106">Permissions</span></span>

<span data-ttu-id="e3280-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3280-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3280-109">Permission type</span></span>                        | <span data-ttu-id="e3280-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3280-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3280-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3280-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3280-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3280-112">Reports.Read.All</span></span> |
| <span data-ttu-id="e3280-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3280-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3280-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3280-114">Not supported.</span></span> |
| <span data-ttu-id="e3280-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3280-115">Application</span></span>                            | <span data-ttu-id="e3280-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3280-116">Reports.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3280-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3280-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getCredentialUsageSummary
```

## <a name="function-parameters"></a><span data-ttu-id="e3280-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e3280-118">Function parameters</span></span>

<span data-ttu-id="e3280-119">Для настройки ответа можно использовать следующий параметр функции.</span><span class="sxs-lookup"><span data-stu-id="e3280-119">You can use the following function parameter to adjust the response.</span></span>

| <span data-ttu-id="e3280-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="e3280-120">Parameter</span></span> | <span data-ttu-id="e3280-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e3280-121">Type</span></span> | <span data-ttu-id="e3280-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e3280-122">Description</span></span> |
|:--------- |:---- |:----------- |
| <span data-ttu-id="e3280-123">period</span><span class="sxs-lookup"><span data-stu-id="e3280-123">period</span></span> | <span data-ttu-id="e3280-124">Строка</span><span class="sxs-lookup"><span data-stu-id="e3280-124">String</span></span> | <span data-ttu-id="e3280-125">Указывает период времени, для которого требуются данные об использовании.</span><span class="sxs-lookup"><span data-stu-id="e3280-125">Specifies the time period for which you need the usage data.</span></span> <span data-ttu-id="e3280-126">Пример: `/reports/getCredentialUsageSummary(period='D30')`.</span><span class="sxs-lookup"><span data-stu-id="e3280-126">For example: `/reports/getCredentialUsageSummary(period='D30')`.</span></span> <span data-ttu-id="e3280-127">Поддерживаемые периоды: `D1` , `D7` , и `D30` .</span><span class="sxs-lookup"><span data-stu-id="e3280-127">Supported periods: `D1`, `D7`, and `D30`.</span></span> <span data-ttu-id="e3280-128">Точка нечувствительна к делу.</span><span class="sxs-lookup"><span data-stu-id="e3280-128">Period is case insensitive.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e3280-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e3280-129">Optional query parameters</span></span>

<span data-ttu-id="e3280-130">Эта функция поддерживает необязательный параметр запроса OData **$filter.**</span><span class="sxs-lookup"><span data-stu-id="e3280-130">This function supports the optional OData query parameter **$filter**.</span></span> <span data-ttu-id="e3280-131">Вы можете **применить $filter** к одному или более из следующих свойств ресурса [credentialUsageSummary.](../resources/credentialusagesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e3280-131">You can apply **$filter** on one or more of the following properties of the [credentialUsageSummary](../resources/credentialusagesummary.md) resource.</span></span>

| <span data-ttu-id="e3280-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3280-132">Properties</span></span> | <span data-ttu-id="e3280-133">Описание и пример</span><span class="sxs-lookup"><span data-stu-id="e3280-133">Description and example</span></span> |
|:---- |:----------- |
| <span data-ttu-id="e3280-134">feature</span><span class="sxs-lookup"><span data-stu-id="e3280-134">feature</span></span> | <span data-ttu-id="e3280-135">Указывает нужный тип данных об использовании (регистрация и сброс).</span><span class="sxs-lookup"><span data-stu-id="e3280-135">Specifies the type of usage data you want (registration vs. reset).</span></span> <span data-ttu-id="e3280-136">Пример: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span><span class="sxs-lookup"><span data-stu-id="e3280-136">For example: `/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'`.</span></span> <span data-ttu-id="e3280-137">Поддерживаемые операторы фильтра: `eq` .</span><span class="sxs-lookup"><span data-stu-id="e3280-137">Supported filter operators: `eq`.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e3280-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3280-138">Request headers</span></span>

| <span data-ttu-id="e3280-139">Имя</span><span class="sxs-lookup"><span data-stu-id="e3280-139">Name</span></span>          | <span data-ttu-id="e3280-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e3280-140">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e3280-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3280-141">Authorization</span></span> | <span data-ttu-id="e3280-142">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e3280-142">Bearer {token}</span></span> |
| <span data-ttu-id="e3280-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3280-143">Content-Type</span></span> | <span data-ttu-id="e3280-144">application/json</span><span class="sxs-lookup"><span data-stu-id="e3280-144">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3280-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3280-145">Request body</span></span>

<span data-ttu-id="e3280-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3280-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3280-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3280-147">Response</span></span>

<span data-ttu-id="e3280-148">В случае успеха этот метод возвращает код отклика и новый объект `200 OK` [коллекции credentialUsageSummary](../resources/credentialusagesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3280-148">If successful, this method returns a `200 OK` response code and a new [credentialUsageSummary](../resources/credentialusagesummary.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3280-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3280-149">Examples</span></span>

<span data-ttu-id="e3280-150">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e3280-150">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e3280-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3280-151">Request</span></span>

<span data-ttu-id="e3280-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3280-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3280-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3280-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getcredentialusagesummary"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getCredentialUsageSummary(period='D30')?$filter=feature eq 'registration'
```
# <a name="c"></a>[<span data-ttu-id="e3280-154">C#</span><span class="sxs-lookup"><span data-stu-id="e3280-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getcredentialusagesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3280-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3280-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getcredentialusagesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3280-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3280-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getcredentialusagesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3280-157">Java</span><span class="sxs-lookup"><span data-stu-id="e3280-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getcredentialusagesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e3280-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3280-158">Response</span></span>

<span data-ttu-id="e3280-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3280-159">The following is an example of the response.</span></span>

> <span data-ttu-id="e3280-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e3280-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e3280-161">Все свойства возвращаются при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e3280-161">All the properties are returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUsageSummary",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getCredentialUsageSummary)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "successfulActivityCount":12345,
      "failureActivityCount": 123,
      "authMethod": "email"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reportRoot: getCredentialUsageSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


