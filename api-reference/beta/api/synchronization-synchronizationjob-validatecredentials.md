---
title: 'synchronizationJob: validateCredentials'
description: Убедитесь, что учетные данные действительны в клиентов.
localization_priority: Normal
ms.openlocfilehash: b78d6f7b3ff197607897fbdce123aa1e7e646afc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834923"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="0be02-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="0be02-103">synchronizationJob: validateCredentials</span></span>

> <span data-ttu-id="0be02-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0be02-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0be02-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0be02-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0be02-106">Убедитесь, что учетные данные действительны в клиентов.</span><span class="sxs-lookup"><span data-stu-id="0be02-106">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0be02-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0be02-107">Permissions</span></span>
<span data-ttu-id="0be02-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0be02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0be02-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0be02-110">Permission type</span></span>                        | <span data-ttu-id="0be02-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0be02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0be02-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0be02-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="0be02-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be02-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0be02-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0be02-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0be02-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0be02-115">Not supported.</span></span> |
|<span data-ttu-id="0be02-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0be02-116">Application</span></span>                            |<span data-ttu-id="0be02-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0be02-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="0be02-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0be02-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="0be02-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0be02-119">Request headers</span></span>
| <span data-ttu-id="0be02-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0be02-120">Name</span></span>       | <span data-ttu-id="0be02-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0be02-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0be02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0be02-122">Authorization</span></span>  | <span data-ttu-id="0be02-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0be02-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0be02-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0be02-124">Request body</span></span>
<span data-ttu-id="0be02-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0be02-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0be02-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="0be02-126">Parameter</span></span>    | <span data-ttu-id="0be02-127">Тип</span><span class="sxs-lookup"><span data-stu-id="0be02-127">Type</span></span>   |<span data-ttu-id="0be02-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0be02-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0be02-129">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="0be02-129">useSavedCredentials</span></span>|<span data-ttu-id="0be02-130">Логический</span><span class="sxs-lookup"><span data-stu-id="0be02-130">Boolean</span></span>|<span data-ttu-id="0be02-131">При `true`, `credentials` параметр игнорируется и проверяются предварительно сохраненных учетных данных (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="0be02-131">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="0be02-132">учетные данные</span><span class="sxs-lookup"><span data-stu-id="0be02-132">credentials</span></span>|<span data-ttu-id="0be02-133">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0be02-133">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="0be02-134">Учетные данные для проверки.</span><span class="sxs-lookup"><span data-stu-id="0be02-134">Credentials to validate.</span></span> <span data-ttu-id="0be02-135">Игнорируется, если `useSavedCredentials` — это параметр `true`.</span><span class="sxs-lookup"><span data-stu-id="0be02-135">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="0be02-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0be02-136">Response</span></span>
<span data-ttu-id="0be02-137">Если проверка прошла успешно, этот метод возвращает `204, No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="0be02-137">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="0be02-138">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0be02-138">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0be02-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0be02-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0be02-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0be02-140">Request</span></span>
<span data-ttu-id="0be02-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0be02-141">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0be02-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="0be02-142">Response</span></span>
<span data-ttu-id="0be02-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0be02-143">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
