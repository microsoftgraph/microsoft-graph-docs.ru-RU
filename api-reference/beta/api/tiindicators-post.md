---
title: Создание индикатора сведении об угрозах
description: Создайте новый tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 14620ff345c5d74075548b17e26bc7923f942da6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050761"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="ce434-103">Создание индикатора сведении об угрозах</span><span class="sxs-lookup"><span data-stu-id="ce434-103">Create threat intelligence indicator</span></span>

<span data-ttu-id="ce434-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce434-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce434-105">Создайте [новый объект tiIndicator.](../resources/tiindicator.md)</span><span class="sxs-lookup"><span data-stu-id="ce434-105">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce434-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce434-106">Permissions</span></span>

<span data-ttu-id="ce434-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce434-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce434-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce434-109">Permission type</span></span>                        | <span data-ttu-id="ce434-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce434-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce434-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce434-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce434-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ce434-112">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="ce434-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce434-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce434-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce434-114">Not supported.</span></span> |
| <span data-ttu-id="ce434-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce434-115">Application</span></span>                            | <span data-ttu-id="ce434-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ce434-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce434-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce434-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="ce434-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce434-118">Request headers</span></span>

| <span data-ttu-id="ce434-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ce434-119">Name</span></span>          | <span data-ttu-id="ce434-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ce434-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ce434-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce434-121">Authorization</span></span> | <span data-ttu-id="ce434-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ce434-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce434-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce434-123">Request body</span></span>

<span data-ttu-id="ce434-124">В корпусе запроса поставляем JSON-представление объекта [tiIndicator,](../resources/tiindicator.md) содержащего [](../resources/tiindicator.md#indicator-observables---network) по крайней мере одно сообщение [электронной](../resources/tiindicator.md#indicator-observables---email)почты, [](../resources/tiindicator.md#indicator-observables---file)файл или сеть, наблюдаемые, и следующие необходимые поля: , , `action` , , `description` `expirationDateTime` `targetProduct` `threatType` `tlpLevel` .</span><span class="sxs-lookup"><span data-stu-id="ce434-124">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable, and the following required fields: `action`, `description`, `expirationDateTime`, `targetProduct`, `threatType`, `tlpLevel`.</span></span> 

## <a name="response"></a><span data-ttu-id="ce434-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce434-125">Response</span></span>

<span data-ttu-id="ce434-126">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект tiIndicator](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce434-126">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce434-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="ce434-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce434-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce434-128">Request</span></span>

<span data-ttu-id="ce434-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce434-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce434-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce434-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ce434-131">C#</span><span class="sxs-lookup"><span data-stu-id="ce434-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce434-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce434-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce434-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce434-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce434-134">Java</span><span class="sxs-lookup"><span data-stu-id="ce434-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tiindicator-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce434-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce434-135">Response</span></span>

<span data-ttu-id="ce434-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ce434-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ce434-137">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ce434-137">The response object shown here might be shortened for readability.</span></span>

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


