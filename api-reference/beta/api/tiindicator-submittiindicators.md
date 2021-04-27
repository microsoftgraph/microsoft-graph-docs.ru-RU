---
title: 'tiIndicator: submitTiIndicators'
description: Upload нескольких индикаторов разведки угроз (TI) в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: ed4ccd5adf087ecf8be69d8d192ae180ec685090
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050782"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="ecc40-103">tiIndicator: submitTiIndicators</span><span class="sxs-lookup"><span data-stu-id="ecc40-103">tiIndicator: submitTiIndicators</span></span>

<span data-ttu-id="ecc40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecc40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecc40-105">Upload нескольких индикаторов разведки угроз (TI) в одном запросе вместо нескольких запросов.</span><span class="sxs-lookup"><span data-stu-id="ecc40-105">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecc40-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecc40-106">Permissions</span></span>

<span data-ttu-id="ecc40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecc40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecc40-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecc40-109">Permission type</span></span> | <span data-ttu-id="ecc40-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecc40-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ecc40-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecc40-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecc40-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ecc40-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="ecc40-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecc40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecc40-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecc40-114">Not supported.</span></span> |
| <span data-ttu-id="ecc40-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ecc40-115">Application</span></span>                            | <span data-ttu-id="ecc40-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ecc40-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecc40-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecc40-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="ecc40-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecc40-118">Request headers</span></span>

| <span data-ttu-id="ecc40-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ecc40-119">Name</span></span>          | <span data-ttu-id="ecc40-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ecc40-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ecc40-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecc40-121">Authorization</span></span> | <span data-ttu-id="ecc40-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ecc40-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecc40-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecc40-123">Request body</span></span>

<span data-ttu-id="ecc40-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ecc40-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ecc40-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="ecc40-125">Parameter</span></span>    | <span data-ttu-id="ecc40-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ecc40-126">Type</span></span>        | <span data-ttu-id="ecc40-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ecc40-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ecc40-128">значение</span><span class="sxs-lookup"><span data-stu-id="ecc40-128">value</span></span>|<span data-ttu-id="ecc40-129">коллекция tiIndicator</span><span class="sxs-lookup"><span data-stu-id="ecc40-129">tiIndicator collection</span></span>| <span data-ttu-id="ecc40-130">Коллекция **tiIndicators** JSON, которая будет создана.</span><span class="sxs-lookup"><span data-stu-id="ecc40-130">JSON collection of **tiIndicators** to be created.</span></span> |

<span data-ttu-id="ecc40-131">Для каждого tiIndicator поставляем JSON-представление объекта [tiIndicator,](../resources/tiindicator.md) [](../resources/tiindicator.md#indicator-observables---file)содержащего [](../resources/tiindicator.md#indicator-observables---network) по крайней мере одну электронную [почту,](../resources/tiindicator.md#indicator-observables---email)файл или сеть, наблюдаемую, и следующие необходимые поля: `action` , , , , `description` `expirationDateTime` `targetProduct` `threatType` `tlpLevel` .</span><span class="sxs-lookup"><span data-stu-id="ecc40-131">For each tiIndicator, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span>

## <a name="response"></a><span data-ttu-id="ecc40-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecc40-132">Response</span></span>

<span data-ttu-id="ecc40-133">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [tiIndicator](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ecc40-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="ecc40-134">При ошибке этот метод возвращает `206 Partial Content` код ответа.</span><span class="sxs-lookup"><span data-stu-id="ecc40-134">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="ecc40-135">Дополнительные [сведения см. в](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) "Ошибках".</span><span class="sxs-lookup"><span data-stu-id="ecc40-135">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="ecc40-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="ecc40-136">Examples</span></span>

<span data-ttu-id="ecc40-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ecc40-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ecc40-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecc40-138">Request</span></span>

<span data-ttu-id="ecc40-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecc40-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ecc40-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecc40-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tiindicator_submittiindicators",
  "isCollection":"true"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators
Content-Type: application/json

{
  "value": [
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1668987+00:00",
      "externalId": "Test--8586509942423126760MS164-0",
      "fileHashType": "sha256",
      "fileHashValue": "b555c45c5b1b01304217e72118d6ca1b14b7013644a078273cea27bbdc1cf9d6",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    },
    {
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
      "expirationDateTime": "2019-03-01T21:44:03.1748779+00:00",
      "externalId": "Test--8586509942423126760MS164-1",
      "fileHashType": "sha256",
      "fileHashValue": "1796b433950990b28d6a22456c9d2b58ced1bdfcdf5f16f7e39d6b9bdca4213b",
      "killChain": [],
      "malwareFamilyNames": [],
      "severity": 0,
      "tags": [],
      "targetProduct": "Azure Sentinel",
      "threatType": "WatchList",
      "tlpLevel": "green",
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ecc40-141">C#</span><span class="sxs-lookup"><span data-stu-id="ecc40-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecc40-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecc40-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecc40-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecc40-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecc40-144">Java</span><span class="sxs-lookup"><span data-stu-id="ecc40-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-submittiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ecc40-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecc40-145">Response</span></span>

<span data-ttu-id="ecc40-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ecc40-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ecc40-147">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ecc40-147">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
      "azureTenantId": "XXXXXXXXXXXXXXXXXXXXX",
      "action": null,
      "additionalInformation": null,
      "activityGroupNames": [],
      "confidence": 0,
      "description": "This is a test indicator for demo purpose. Take no action on any observables set in this indicator.",
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator: submitTiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


