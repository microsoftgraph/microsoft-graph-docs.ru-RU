---
title: Создание индикатора для логики операций с угрозами
description: Создание нового Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 46af7c54c5af55ad44e04a961171530cc4a74fa3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409249"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="dc43a-103">Создание индикатора для логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="dc43a-103">Create threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc43a-104">Создание нового объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="dc43a-104">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc43a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc43a-105">Permissions</span></span>

<span data-ttu-id="dc43a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc43a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc43a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc43a-108">Permission type</span></span>                        | <span data-ttu-id="dc43a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc43a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dc43a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc43a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc43a-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="dc43a-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="dc43a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc43a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc43a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc43a-113">Not supported.</span></span> |
| <span data-ttu-id="dc43a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc43a-114">Application</span></span>                            | <span data-ttu-id="dc43a-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="dc43a-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc43a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc43a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="dc43a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc43a-117">Request headers</span></span>

| <span data-ttu-id="dc43a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dc43a-118">Name</span></span>          | <span data-ttu-id="dc43a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dc43a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dc43a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc43a-120">Authorization</span></span> | <span data-ttu-id="dc43a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dc43a-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc43a-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc43a-122">Request body</span></span>

<span data-ttu-id="dc43a-123">В тексте запроса добавьте представление объекта [тииндикатор](../resources/tiindicator.md) в формате JSON, содержащий хотя бы один наблюдаемый [адрес электронной почты](../resources/tiindicator.md#indicator-observables---email), [файл](../resources/tiindicator.md#indicator-observables---file)или [сеть](../resources/tiindicator.md#indicator-observables---network) .</span><span class="sxs-lookup"><span data-stu-id="dc43a-123">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable.</span></span>

## <a name="response"></a><span data-ttu-id="dc43a-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc43a-124">Response</span></span>

<span data-ttu-id="dc43a-125">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc43a-125">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc43a-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="dc43a-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc43a-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc43a-127">Request</span></span>

<span data-ttu-id="dc43a-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc43a-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dc43a-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc43a-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tiindicator_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators
Content-type: application/json

{
  "action": "alert",
  "activityGroupNames": [],
  "confidence": 0,
  "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
  "expirationDateTime": "2019-03-01T21:43:37.5031462+00:00",
  "externalId": "Test--8586509942679764298MS501",
  "fileHashType": "sha256",
  "fileHashValue": "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313",
  "killChain": [],
  "malwareFamilyNames": [],
  "severity": 0,
  "tags": [],
  "targetProduct": "Azure Sentinel",
  "threatType": "WatchList",
  "tlpLevel": "green"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc43a-130">C#</span><span class="sxs-lookup"><span data-stu-id="dc43a-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc43a-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc43a-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc43a-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dc43a-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc43a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc43a-133">Response</span></span>

<span data-ttu-id="dc43a-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dc43a-134">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="dc43a-135">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dc43a-135">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dc43a-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc43a-136">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXX",
    "action": "alert",
    "additionalInformation": null,
    "activityGroupNames": [],
    "confidence": 0,
    "description": "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
