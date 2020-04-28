---
title: 'Тииндикатор: Субмиттииндикаторс'
description: Отправьте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0fa3fcfad09b345cc5dac741f71b63022de38571
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452367"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="9f1d0-103">Тииндикатор: Субмиттииндикаторс</span><span class="sxs-lookup"><span data-stu-id="9f1d0-103">tiIndicator: submitTiIndicators</span></span>

<span data-ttu-id="9f1d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f1d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f1d0-105">Отправьте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-105">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f1d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f1d0-106">Permissions</span></span>

<span data-ttu-id="9f1d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f1d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f1d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f1d0-109">Permission type</span></span> | <span data-ttu-id="9f1d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f1d0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9f1d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f1d0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f1d0-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9f1d0-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="9f1d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f1d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f1d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-114">Not supported.</span></span> |
| <span data-ttu-id="9f1d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f1d0-115">Application</span></span>                            | <span data-ttu-id="9f1d0-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="9f1d0-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f1d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f1d0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="9f1d0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f1d0-118">Request headers</span></span>

| <span data-ttu-id="9f1d0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f1d0-119">Name</span></span>          | <span data-ttu-id="9f1d0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9f1d0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9f1d0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f1d0-121">Authorization</span></span> | <span data-ttu-id="9f1d0-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9f1d0-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f1d0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f1d0-123">Request body</span></span>

<span data-ttu-id="9f1d0-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9f1d0-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="9f1d0-125">Parameter</span></span>    | <span data-ttu-id="9f1d0-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9f1d0-126">Type</span></span>        | <span data-ttu-id="9f1d0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9f1d0-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9f1d0-128">значение</span><span class="sxs-lookup"><span data-stu-id="9f1d0-128">value</span></span>|<span data-ttu-id="9f1d0-129">Коллекция Тииндикатор</span><span class="sxs-lookup"><span data-stu-id="9f1d0-129">tiIndicator collection</span></span>| <span data-ttu-id="9f1d0-130">Коллекция объектов **тииндикаторс** , которую необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-130">JSON collection of **tiIndicators** to be created.</span></span> |

<span data-ttu-id="9f1d0-131">Для каждого Тииндикатор добавьте представление объекта [тииндикатор](../resources/tiindicator.md) в [формате](../resources/tiindicator.md#indicator-observables---file)JSON, содержащий хотя бы один наблюдаемый [адрес электронной почты](../resources/tiindicator.md#indicator-observables---email), файл или [сеть](../resources/tiindicator.md#indicator-observables---network) , а также следующие обязательные поля `action`: `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`,.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-131">For each tiIndicator, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span>

## <a name="response"></a><span data-ttu-id="9f1d0-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f1d0-132">Response</span></span>

<span data-ttu-id="9f1d0-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="9f1d0-134">При возникновении ошибки этот метод возвращает код `206 Partial Content` отклика.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-134">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="9f1d0-135">Дополнительные сведения см. в разделе [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) .</span><span class="sxs-lookup"><span data-stu-id="9f1d0-135">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="9f1d0-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f1d0-136">Examples</span></span>

<span data-ttu-id="9f1d0-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9f1d0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f1d0-138">Request</span></span>

<span data-ttu-id="9f1d0-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f1d0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f1d0-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9f1d0-141">C#</span><span class="sxs-lookup"><span data-stu-id="9f1d0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f1d0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f1d0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f1d0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f1d0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9f1d0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f1d0-144">Response</span></span>

<span data-ttu-id="9f1d0-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="9f1d0-146">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9f1d0-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f1d0-147">All the properties will be returned from an actual call.</span></span>

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
