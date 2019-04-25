---
title: 'Синчронизатионжоб: Валидатекредентиалс'
description: Убедитесь, что учетные данные действительны в клиенте.
localization_priority: Normal
ms.openlocfilehash: 122d673e89f15697b2fdeefbcefb516cf9ad89ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537141"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="b93c7-103">Синчронизатионжоб: Валидатекредентиалс</span><span class="sxs-lookup"><span data-stu-id="b93c7-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b93c7-104">Убедитесь, что учетные данные действительны в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b93c7-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b93c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b93c7-105">Permissions</span></span>
<span data-ttu-id="b93c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b93c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b93c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b93c7-108">Permission type</span></span>                        | <span data-ttu-id="b93c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b93c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b93c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b93c7-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="b93c7-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b93c7-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b93c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b93c7-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b93c7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b93c7-113">Not supported.</span></span> |
|<span data-ttu-id="b93c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b93c7-114">Application</span></span>                            |<span data-ttu-id="b93c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b93c7-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="b93c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b93c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="b93c7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b93c7-117">Request headers</span></span>
| <span data-ttu-id="b93c7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b93c7-118">Name</span></span>       | <span data-ttu-id="b93c7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b93c7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b93c7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b93c7-120">Authorization</span></span>  | <span data-ttu-id="b93c7-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b93c7-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b93c7-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b93c7-122">Request body</span></span>
<span data-ttu-id="b93c7-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b93c7-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b93c7-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="b93c7-124">Parameter</span></span>    | <span data-ttu-id="b93c7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b93c7-125">Type</span></span>   |<span data-ttu-id="b93c7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b93c7-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b93c7-127">Усесаведкредентиалс</span><span class="sxs-lookup"><span data-stu-id="b93c7-127">useSavedCredentials</span></span>|<span data-ttu-id="b93c7-128">Логический</span><span class="sxs-lookup"><span data-stu-id="b93c7-128">Boolean</span></span>|<span data-ttu-id="b93c7-129">Когда `true` `credentials` параметр будет игнорироваться и будут проверены ранее сохраненные учетные данные (если они есть).</span><span class="sxs-lookup"><span data-stu-id="b93c7-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="b93c7-130">записей</span><span class="sxs-lookup"><span data-stu-id="b93c7-130">credentials</span></span>|<span data-ttu-id="b93c7-131">Коллекция [синчронизатионсекреткэйстрингвалуепаир](../resources/synchronization-secretkeystringvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b93c7-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="b93c7-132">Учетные данные для проверки.</span><span class="sxs-lookup"><span data-stu-id="b93c7-132">Credentials to validate.</span></span> <span data-ttu-id="b93c7-133">Игнорируется, `useSavedCredentials` если параметр `true`имеет значение.</span><span class="sxs-lookup"><span data-stu-id="b93c7-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="b93c7-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b93c7-134">Response</span></span>
<span data-ttu-id="b93c7-135">Если проверка прошла успешно, этот метод возвращает `204, No Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="b93c7-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="b93c7-136">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b93c7-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b93c7-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b93c7-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b93c7-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b93c7-138">Request</span></span>
<span data-ttu-id="b93c7-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b93c7-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b93c7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b93c7-140">Response</span></span>
<span data-ttu-id="b93c7-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b93c7-141">The following is an example of the response.</span></span> 
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
