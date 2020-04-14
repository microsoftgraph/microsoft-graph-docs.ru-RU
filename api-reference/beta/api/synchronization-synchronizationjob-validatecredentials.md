---
title: 'Синчронизатионжоб: Валидатекредентиалс'
description: Убедитесь, что учетные данные действительны в клиенте.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc61dd5eb9d5e012f0fce672eac4f330eb460df3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437514"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="2e0d4-103">Синчронизатионжоб: Валидатекредентиалс</span><span class="sxs-lookup"><span data-stu-id="2e0d4-103">synchronizationJob: validateCredentials</span></span>

<span data-ttu-id="2e0d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e0d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e0d4-105">Убедитесь, что учетные данные действительны в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-105">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e0d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e0d4-106">Permissions</span></span>
<span data-ttu-id="2e0d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e0d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e0d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e0d4-109">Permission type</span></span>                        | <span data-ttu-id="2e0d4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e0d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e0d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e0d4-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="2e0d4-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e0d4-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2e0d4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e0d4-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2e0d4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-114">Not supported.</span></span> |
|<span data-ttu-id="2e0d4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e0d4-115">Application</span></span>                            |<span data-ttu-id="2e0d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="2e0d4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e0d4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="2e0d4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e0d4-118">Request headers</span></span>
| <span data-ttu-id="2e0d4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2e0d4-119">Name</span></span>       | <span data-ttu-id="2e0d4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2e0d4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2e0d4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e0d4-121">Authorization</span></span>  | <span data-ttu-id="2e0d4-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2e0d4-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e0d4-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e0d4-123">Request body</span></span>
<span data-ttu-id="2e0d4-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e0d4-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="2e0d4-125">Parameter</span></span>    | <span data-ttu-id="2e0d4-126">Тип</span><span class="sxs-lookup"><span data-stu-id="2e0d4-126">Type</span></span>   |<span data-ttu-id="2e0d4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="2e0d4-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e0d4-128">усесаведкредентиалс</span><span class="sxs-lookup"><span data-stu-id="2e0d4-128">useSavedCredentials</span></span>|<span data-ttu-id="2e0d4-129">Логическое</span><span class="sxs-lookup"><span data-stu-id="2e0d4-129">Boolean</span></span>|<span data-ttu-id="2e0d4-130">Когда `true` `credentials` параметр будет игнорироваться и будут проверены ранее сохраненные учетные данные (если они есть).</span><span class="sxs-lookup"><span data-stu-id="2e0d4-130">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="2e0d4-131">записей</span><span class="sxs-lookup"><span data-stu-id="2e0d4-131">credentials</span></span>|<span data-ttu-id="2e0d4-132">Коллекция [синчронизатионсекреткэйстрингвалуепаир](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2e0d4-132">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="2e0d4-133">Учетные данные для проверки.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-133">Credentials to validate.</span></span> <span data-ttu-id="2e0d4-134">Игнорируется, `useSavedCredentials` если параметр `true`имеет значение.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-134">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="2e0d4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e0d4-135">Response</span></span>
<span data-ttu-id="2e0d4-136">Если проверка прошла успешно, этот метод возвращает `204, No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-136">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="2e0d4-137">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e0d4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2e0d4-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2e0d4-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e0d4-139">Request</span></span>
<span data-ttu-id="2e0d4-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e0d4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e0d4-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2e0d4-142">C#</span><span class="sxs-lookup"><span data-stu-id="2e0d4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e0d4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e0d4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e0d4-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e0d4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2e0d4-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e0d4-145">Response</span></span>
<span data-ttu-id="2e0d4-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e0d4-146">The following is an example of the response.</span></span> 
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
