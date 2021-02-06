---
title: 'synchronizationJob: validateCredentials'
description: Проверьте, действительны ли учетные данные в клиенте.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 4f36764ca7d6787629299261e6ec42c9454ddc46
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132071"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="c4353-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="c4353-103">synchronizationJob: validateCredentials</span></span>

<span data-ttu-id="c4353-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4353-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4353-105">Проверьте, действительны ли учетные данные в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c4353-105">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4353-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4353-106">Permissions</span></span>
<span data-ttu-id="c4353-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4353-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4353-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4353-109">Permission type</span></span>                        | <span data-ttu-id="c4353-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4353-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4353-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4353-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="c4353-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4353-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c4353-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4353-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c4353-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4353-114">Not supported.</span></span> |
|<span data-ttu-id="c4353-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4353-115">Application</span></span>                            |<span data-ttu-id="c4353-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4353-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="c4353-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4353-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="c4353-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4353-118">Request headers</span></span>
| <span data-ttu-id="c4353-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4353-119">Name</span></span>       | <span data-ttu-id="c4353-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4353-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4353-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4353-121">Authorization</span></span>  | <span data-ttu-id="c4353-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c4353-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4353-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4353-123">Request body</span></span>
<span data-ttu-id="c4353-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c4353-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4353-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4353-125">Parameter</span></span>    | <span data-ttu-id="c4353-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c4353-126">Type</span></span>   |<span data-ttu-id="c4353-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c4353-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4353-128">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="c4353-128">useSavedCredentials</span></span>|<span data-ttu-id="c4353-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4353-129">Boolean</span></span>|<span data-ttu-id="c4353-130">Если параметр будет игнорироваться, а ранее сохраненные учетные данные (если таковые есть) будут `true` `credentials` проверены.</span><span class="sxs-lookup"><span data-stu-id="c4353-130">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="c4353-131">credentials</span><span class="sxs-lookup"><span data-stu-id="c4353-131">credentials</span></span>|<span data-ttu-id="c4353-132">[Коллекция synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c4353-132">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="c4353-133">Учетные данные для проверки.</span><span class="sxs-lookup"><span data-stu-id="c4353-133">Credentials to validate.</span></span> <span data-ttu-id="c4353-134">Игнорируется, если `useSavedCredentials` параметр имеет . `true`</span><span class="sxs-lookup"><span data-stu-id="c4353-134">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="c4353-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4353-135">Response</span></span>
<span data-ttu-id="c4353-136">Если проверка прошла успешно, этот метод возвращает `204, No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="c4353-136">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="c4353-137">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c4353-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4353-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c4353-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c4353-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4353-139">Request</span></span>
<span data-ttu-id="c4353-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4353-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4353-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4353-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_validatecredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
Content-type: application/json
Content-length: 218

{ 
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="c4353-142">C#</span><span class="sxs-lookup"><span data-stu-id="c4353-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4353-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4353-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4353-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4353-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4353-145">Java</span><span class="sxs-lookup"><span data-stu-id="c4353-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-validatecredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4353-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4353-146">Response</span></span>
<span data-ttu-id="c4353-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c4353-147">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


