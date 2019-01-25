---
title: 'synchronizationJob: validateCredentials'
description: Убедитесь, что учетные данные действительны в клиентов.
localization_priority: Normal
ms.openlocfilehash: 122d673e89f15697b2fdeefbcefb516cf9ad89ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519005"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="b9b93-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="b9b93-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9b93-104">Убедитесь, что учетные данные действительны в клиентов.</span><span class="sxs-lookup"><span data-stu-id="b9b93-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9b93-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9b93-105">Permissions</span></span>
<span data-ttu-id="b9b93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9b93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9b93-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9b93-108">Permission type</span></span>                        | <span data-ttu-id="b9b93-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9b93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9b93-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9b93-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="b9b93-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9b93-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b9b93-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9b93-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b9b93-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9b93-113">Not supported.</span></span> |
|<span data-ttu-id="b9b93-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9b93-114">Application</span></span>                            |<span data-ttu-id="b9b93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9b93-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="b9b93-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9b93-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="b9b93-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9b93-117">Request headers</span></span>
| <span data-ttu-id="b9b93-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b9b93-118">Name</span></span>       | <span data-ttu-id="b9b93-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b9b93-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9b93-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9b93-120">Authorization</span></span>  | <span data-ttu-id="b9b93-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b9b93-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9b93-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9b93-122">Request body</span></span>
<span data-ttu-id="b9b93-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b9b93-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9b93-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="b9b93-124">Parameter</span></span>    | <span data-ttu-id="b9b93-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b9b93-125">Type</span></span>   |<span data-ttu-id="b9b93-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b9b93-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9b93-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="b9b93-127">useSavedCredentials</span></span>|<span data-ttu-id="b9b93-128">Логическое</span><span class="sxs-lookup"><span data-stu-id="b9b93-128">Boolean</span></span>|<span data-ttu-id="b9b93-129">При `true`, `credentials` параметр игнорируется и проверяются предварительно сохраненных учетных данных (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="b9b93-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="b9b93-130">Credentials</span><span class="sxs-lookup"><span data-stu-id="b9b93-130">credentials</span></span>|<span data-ttu-id="b9b93-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b9b93-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="b9b93-132">Учетные данные для проверки.</span><span class="sxs-lookup"><span data-stu-id="b9b93-132">Credentials to validate.</span></span> <span data-ttu-id="b9b93-133">Игнорируется, если `useSavedCredentials` — это параметр `true`.</span><span class="sxs-lookup"><span data-stu-id="b9b93-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="b9b93-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9b93-134">Response</span></span>
<span data-ttu-id="b9b93-135">Если проверка прошла успешно, этот метод возвращает `204, No Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="b9b93-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="b9b93-136">Он не возвращает все действия в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9b93-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9b93-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b9b93-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b9b93-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9b93-138">Request</span></span>
<span data-ttu-id="b9b93-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9b93-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b9b93-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9b93-140">Response</span></span>
<span data-ttu-id="b9b93-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9b93-141">The following is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
