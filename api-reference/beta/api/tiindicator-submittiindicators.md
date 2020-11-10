---
title: 'Тииндикатор: Субмиттииндикаторс'
description: Отправьте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: bb3542c678fbee89a4de293585d31094502c857e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975869"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="de657-103">Тииндикатор: Субмиттииндикаторс</span><span class="sxs-lookup"><span data-stu-id="de657-103">tiIndicator: submitTiIndicators</span></span>

<span data-ttu-id="de657-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de657-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de657-105">Отправьте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.</span><span class="sxs-lookup"><span data-stu-id="de657-105">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="de657-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de657-106">Permissions</span></span>

<span data-ttu-id="de657-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de657-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de657-109">Permission type</span></span> | <span data-ttu-id="de657-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de657-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de657-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de657-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de657-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="de657-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="de657-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de657-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de657-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de657-114">Not supported.</span></span> |
| <span data-ttu-id="de657-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="de657-115">Application</span></span>                            | <span data-ttu-id="de657-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="de657-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="de657-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de657-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="de657-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de657-118">Request headers</span></span>

| <span data-ttu-id="de657-119">Имя</span><span class="sxs-lookup"><span data-stu-id="de657-119">Name</span></span>          | <span data-ttu-id="de657-120">Описание</span><span class="sxs-lookup"><span data-stu-id="de657-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="de657-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de657-121">Authorization</span></span> | <span data-ttu-id="de657-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="de657-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="de657-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de657-123">Request body</span></span>

<span data-ttu-id="de657-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="de657-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="de657-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="de657-125">Parameter</span></span>    | <span data-ttu-id="de657-126">Тип</span><span class="sxs-lookup"><span data-stu-id="de657-126">Type</span></span>        | <span data-ttu-id="de657-127">Описание</span><span class="sxs-lookup"><span data-stu-id="de657-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de657-128">значение</span><span class="sxs-lookup"><span data-stu-id="de657-128">value</span></span>|<span data-ttu-id="de657-129">Коллекция Тииндикатор</span><span class="sxs-lookup"><span data-stu-id="de657-129">tiIndicator collection</span></span>| <span data-ttu-id="de657-130">Коллекция объектов **тииндикаторс** , которую необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="de657-130">JSON collection of **tiIndicators** to be created.</span></span> |

<span data-ttu-id="de657-131">Для каждого Тииндикатор добавьте представление объекта [тииндикатор](../resources/tiindicator.md) в формате JSON, содержащий хотя бы один наблюдаемый [адрес электронной почты](../resources/tiindicator.md#indicator-observables---email), [файл](../resources/tiindicator.md#indicator-observables---file)или [сеть](../resources/tiindicator.md#indicator-observables---network) , а также следующие обязательные поля:,, `action` ,, `description` `expirationDateTime` `targetProduct` `threatType` , `tlpLevel` .</span><span class="sxs-lookup"><span data-stu-id="de657-131">For each tiIndicator, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span>

## <a name="response"></a><span data-ttu-id="de657-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="de657-132">Response</span></span>

<span data-ttu-id="de657-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de657-133">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>  <span data-ttu-id="de657-134">При возникновении ошибки этот метод возвращает `206 Partial Content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="de657-134">If there is an error, this method returns a `206 Partial Content` response code.</span></span>  <span data-ttu-id="de657-135">Дополнительные сведения см. в разделе [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) .</span><span class="sxs-lookup"><span data-stu-id="de657-135">See [Errors](../resources/security-error-codes.md#threat-indicator-bulk-action-errors) for more information.</span></span>

## <a name="examples"></a><span data-ttu-id="de657-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="de657-136">Examples</span></span>

<span data-ttu-id="de657-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="de657-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="de657-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="de657-138">Request</span></span>

<span data-ttu-id="de657-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de657-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de657-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="de657-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="de657-141">C#</span><span class="sxs-lookup"><span data-stu-id="de657-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tiindicator-submittiindicators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de657-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de657-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tiindicator-submittiindicators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de657-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de657-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tiindicator-submittiindicators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de657-144">Java</span><span class="sxs-lookup"><span data-stu-id="de657-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tiindicator-submittiindicators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de657-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="de657-145">Response</span></span>

<span data-ttu-id="de657-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de657-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="de657-147">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de657-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="de657-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de657-148">All the properties will be returned from an actual call.</span></span>

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


