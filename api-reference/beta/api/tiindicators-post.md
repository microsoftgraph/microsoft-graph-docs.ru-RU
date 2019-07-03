---
title: Создание индикатора для логики операций с угрозами
description: Создание нового Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 208458da18f637b02da7f911289787203b7b5677
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35451299"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="be6c4-103">Создание индикатора для логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="be6c4-103">Create threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be6c4-104">Создание нового объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="be6c4-104">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be6c4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be6c4-105">Permissions</span></span>

<span data-ttu-id="be6c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be6c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be6c4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be6c4-108">Permission type</span></span>                        | <span data-ttu-id="be6c4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be6c4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be6c4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be6c4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="be6c4-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="be6c4-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="be6c4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be6c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be6c4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be6c4-113">Not supported.</span></span> |
| <span data-ttu-id="be6c4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be6c4-114">Application</span></span>                            | <span data-ttu-id="be6c4-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="be6c4-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="be6c4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be6c4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="be6c4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be6c4-117">Request headers</span></span>

| <span data-ttu-id="be6c4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="be6c4-118">Name</span></span>          | <span data-ttu-id="be6c4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="be6c4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="be6c4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be6c4-120">Authorization</span></span> | <span data-ttu-id="be6c4-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="be6c4-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="be6c4-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be6c4-122">Request body</span></span>

<span data-ttu-id="be6c4-123">В тексте запроса добавьте представление объекта [тииндикатор](../resources/tiindicator.md) в формате JSON, содержащий хотя бы один наблюдаемый [адрес электронной почты](../resources/tiindicator.md#indicator-observables---email), [файл](../resources/tiindicator.md#indicator-observables---file)или [сеть](../resources/tiindicator.md#indicator-observables---network) .</span><span class="sxs-lookup"><span data-stu-id="be6c4-123">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one [email](../resources/tiindicator.md#indicator-observables---email), [file](../resources/tiindicator.md#indicator-observables---file), or [network](../resources/tiindicator.md#indicator-observables---network) observable.</span></span>

## <a name="response"></a><span data-ttu-id="be6c4-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="be6c4-124">Response</span></span>

<span data-ttu-id="be6c4-125">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be6c4-125">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be6c4-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="be6c4-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be6c4-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="be6c4-127">Request</span></span>

<span data-ttu-id="be6c4-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be6c4-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="be6c4-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="be6c4-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="be6c4-130">C#</span><span class="sxs-lookup"><span data-stu-id="be6c4-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tiindicator-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be6c4-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="be6c4-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tiindicator-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="be6c4-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="be6c4-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tiindicator-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="be6c4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="be6c4-133">Response</span></span>

<span data-ttu-id="be6c4-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="be6c4-134">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="be6c4-135">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="be6c4-135">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="be6c4-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be6c4-136">All the properties will be returned from an actual call.</span></span>

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
