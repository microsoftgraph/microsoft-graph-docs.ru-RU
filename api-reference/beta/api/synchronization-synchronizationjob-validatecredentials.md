---
title: 'synchronizationJob: validateCredentials'
description: Проверьте, допустимы ли учетные данные в клиенте.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 650cbc18aeb0dc28ef732c4065aa67d19f1a710f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787171"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="c5365-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="c5365-103">synchronizationJob: validateCredentials</span></span>

<span data-ttu-id="c5365-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5365-105">Проверьте, допустимы ли учетные данные в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c5365-105">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5365-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5365-106">Permissions</span></span>
<span data-ttu-id="c5365-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5365-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5365-109">Permission type</span></span>                        | <span data-ttu-id="c5365-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5365-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5365-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5365-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="c5365-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5365-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c5365-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5365-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c5365-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5365-114">Not supported.</span></span> |
|<span data-ttu-id="c5365-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c5365-115">Application</span></span>                            |<span data-ttu-id="c5365-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5365-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c5365-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5365-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="c5365-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5365-118">Request headers</span></span>
| <span data-ttu-id="c5365-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c5365-119">Name</span></span>       | <span data-ttu-id="c5365-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c5365-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c5365-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5365-121">Authorization</span></span>  | <span data-ttu-id="c5365-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c5365-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5365-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5365-123">Request body</span></span>
<span data-ttu-id="c5365-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c5365-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5365-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="c5365-125">Parameter</span></span>    | <span data-ttu-id="c5365-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c5365-126">Type</span></span>   |<span data-ttu-id="c5365-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c5365-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5365-128">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="c5365-128">useSavedCredentials</span></span>|<span data-ttu-id="c5365-129">Логический</span><span class="sxs-lookup"><span data-stu-id="c5365-129">Boolean</span></span>|<span data-ttu-id="c5365-130">Когда параметр будет проигнорирован, а ранее сохраненные учетные данные (если таковые есть) будут `true` `credentials` проверены.</span><span class="sxs-lookup"><span data-stu-id="c5365-130">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="c5365-131">учетные данные</span><span class="sxs-lookup"><span data-stu-id="c5365-131">credentials</span></span>|<span data-ttu-id="c5365-132">[синхронизацияSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) коллекция</span><span class="sxs-lookup"><span data-stu-id="c5365-132">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="c5365-133">Учетные данные для проверки.</span><span class="sxs-lookup"><span data-stu-id="c5365-133">Credentials to validate.</span></span> <span data-ttu-id="c5365-134">Игнорируется при `useSavedCredentials` параметре `true` .</span><span class="sxs-lookup"><span data-stu-id="c5365-134">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="c5365-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5365-135">Response</span></span>
<span data-ttu-id="c5365-136">Если проверка будет успешной, этот метод возвращает `204, No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="c5365-136">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="c5365-137">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c5365-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5365-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c5365-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c5365-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5365-139">Request</span></span>
<span data-ttu-id="c5365-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5365-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5365-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5365-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c5365-142">C#</span><span class="sxs-lookup"><span data-stu-id="c5365-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5365-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5365-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5365-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5365-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5365-145">Java</span><span class="sxs-lookup"><span data-stu-id="c5365-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-validatecredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c5365-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5365-146">Response</span></span>
<span data-ttu-id="c5365-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c5365-147">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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


