---
title: 'Синчронизатионжоб: Валидатекредентиалс'
description: Убедитесь, что учетные данные действительны в клиенте.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c12f2d810841fb3f168e1196d466f6162ad4e1a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982706"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="9eb8f-103">Синчронизатионжоб: Валидатекредентиалс</span><span class="sxs-lookup"><span data-stu-id="9eb8f-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9eb8f-104">Убедитесь, что учетные данные действительны в клиенте.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9eb8f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9eb8f-105">Permissions</span></span>
<span data-ttu-id="9eb8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eb8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eb8f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9eb8f-108">Permission type</span></span>                        | <span data-ttu-id="9eb8f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9eb8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9eb8f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9eb8f-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="9eb8f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eb8f-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9eb8f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9eb8f-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9eb8f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-113">Not supported.</span></span> |
|<span data-ttu-id="9eb8f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9eb8f-114">Application</span></span>                            |<span data-ttu-id="9eb8f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="9eb8f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9eb8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="9eb8f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9eb8f-117">Request headers</span></span>
| <span data-ttu-id="9eb8f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9eb8f-118">Name</span></span>       | <span data-ttu-id="9eb8f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9eb8f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9eb8f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9eb8f-120">Authorization</span></span>  | <span data-ttu-id="9eb8f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9eb8f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9eb8f-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9eb8f-122">Request body</span></span>
<span data-ttu-id="9eb8f-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9eb8f-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="9eb8f-124">Parameter</span></span>    | <span data-ttu-id="9eb8f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9eb8f-125">Type</span></span>   |<span data-ttu-id="9eb8f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9eb8f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9eb8f-127">Усесаведкредентиалс</span><span class="sxs-lookup"><span data-stu-id="9eb8f-127">useSavedCredentials</span></span>|<span data-ttu-id="9eb8f-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eb8f-128">Boolean</span></span>|<span data-ttu-id="9eb8f-129">Когда `true` `credentials` параметр будет игнорироваться и будут проверены ранее сохраненные учетные данные (если они есть).</span><span class="sxs-lookup"><span data-stu-id="9eb8f-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="9eb8f-130">записей</span><span class="sxs-lookup"><span data-stu-id="9eb8f-130">credentials</span></span>|<span data-ttu-id="9eb8f-131">Коллекция [синчронизатионсекреткэйстрингвалуепаир](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9eb8f-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="9eb8f-132">Учетные данные для проверки.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-132">Credentials to validate.</span></span> <span data-ttu-id="9eb8f-133">Игнорируется, `useSavedCredentials` если параметр `true`имеет значение.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="9eb8f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eb8f-134">Response</span></span>
<span data-ttu-id="9eb8f-135">Если проверка прошла успешно, этот метод возвращает `204, No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="9eb8f-136">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eb8f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9eb8f-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9eb8f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9eb8f-138">Request</span></span>
<span data-ttu-id="9eb8f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9eb8f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9eb8f-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9eb8f-141">C#</span><span class="sxs-lookup"><span data-stu-id="9eb8f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9eb8f-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="9eb8f-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9eb8f-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9eb8f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9eb8f-144">Java</span><span class="sxs-lookup"><span data-stu-id="9eb8f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-validatecredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9eb8f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eb8f-145">Response</span></span>
<span data-ttu-id="9eb8f-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9eb8f-146">The following is an example of the response.</span></span> 
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
