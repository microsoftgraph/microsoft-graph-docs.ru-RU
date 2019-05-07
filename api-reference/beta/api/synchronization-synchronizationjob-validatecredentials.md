---
title: 'Синчронизатионжоб: Валидатекредентиалс'
description: Убедитесь, что учетные данные действительны в клиенте.
localization_priority: Normal
ms.openlocfilehash: b533305f622ddb5249fb64727979cafb6fbbc56a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638006"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="0373f-103">Синчронизатионжоб: Валидатекредентиалс</span><span class="sxs-lookup"><span data-stu-id="0373f-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0373f-104">Убедитесь, что учетные данные действительны в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0373f-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0373f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0373f-105">Permissions</span></span>
<span data-ttu-id="0373f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0373f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0373f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0373f-108">Permission type</span></span>                        | <span data-ttu-id="0373f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0373f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0373f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0373f-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="0373f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0373f-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0373f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0373f-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0373f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0373f-113">Not supported.</span></span> |
|<span data-ttu-id="0373f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0373f-114">Application</span></span>                            |<span data-ttu-id="0373f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0373f-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="0373f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0373f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="0373f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0373f-117">Request headers</span></span>
| <span data-ttu-id="0373f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0373f-118">Name</span></span>       | <span data-ttu-id="0373f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0373f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0373f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0373f-120">Authorization</span></span>  | <span data-ttu-id="0373f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0373f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0373f-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0373f-122">Request body</span></span>
<span data-ttu-id="0373f-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0373f-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0373f-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="0373f-124">Parameter</span></span>    | <span data-ttu-id="0373f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0373f-125">Type</span></span>   |<span data-ttu-id="0373f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0373f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0373f-127">Усесаведкредентиалс</span><span class="sxs-lookup"><span data-stu-id="0373f-127">useSavedCredentials</span></span>|<span data-ttu-id="0373f-128">Логический</span><span class="sxs-lookup"><span data-stu-id="0373f-128">Boolean</span></span>|<span data-ttu-id="0373f-129">Когда `true` `credentials` параметр будет игнорироваться и будут проверены ранее сохраненные учетные данные (если они есть).</span><span class="sxs-lookup"><span data-stu-id="0373f-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="0373f-130">записей</span><span class="sxs-lookup"><span data-stu-id="0373f-130">credentials</span></span>|<span data-ttu-id="0373f-131">Коллекция [синчронизатионсекреткэйстрингвалуепаир](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0373f-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="0373f-132">Учетные данные для проверки.</span><span class="sxs-lookup"><span data-stu-id="0373f-132">Credentials to validate.</span></span> <span data-ttu-id="0373f-133">Игнорируется, `useSavedCredentials` если параметр `true`имеет значение.</span><span class="sxs-lookup"><span data-stu-id="0373f-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="0373f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0373f-134">Response</span></span>
<span data-ttu-id="0373f-135">Если проверка прошла успешно, этот метод возвращает `204, No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="0373f-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="0373f-136">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0373f-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0373f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0373f-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0373f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0373f-138">Request</span></span>
<span data-ttu-id="0373f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0373f-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0373f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0373f-140">Response</span></span>
<span data-ttu-id="0373f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0373f-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0373f-142">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="0373f-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0373f-143">Языках</span><span class="sxs-lookup"><span data-stu-id="0373f-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0373f-144">Язык</span><span class="sxs-lookup"><span data-stu-id="0373f-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
