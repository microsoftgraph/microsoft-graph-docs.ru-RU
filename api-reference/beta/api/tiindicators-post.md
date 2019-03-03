---
title: Создание индикатора для логики операций с угрозами
description: Создание нового Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 893af5a56c517cbd4c100cbaa767aa42c70d74e2
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366982"
---
# <a name="create-threat-intelligence-indicator"></a><span data-ttu-id="5983a-103">Создание индикатора для логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="5983a-103">Create threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5983a-104">Создание нового объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="5983a-104">Create a new [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5983a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5983a-105">Permissions</span></span>

<span data-ttu-id="5983a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5983a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5983a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5983a-108">Permission type</span></span>                        | <span data-ttu-id="5983a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5983a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5983a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5983a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5983a-111">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="5983a-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="5983a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5983a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5983a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5983a-113">Not supported.</span></span> |
| <span data-ttu-id="5983a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5983a-114">Application</span></span>                            | <span data-ttu-id="5983a-115">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="5983a-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="5983a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5983a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="5983a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5983a-117">Request headers</span></span>

| <span data-ttu-id="5983a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5983a-118">Name</span></span>          | <span data-ttu-id="5983a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5983a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5983a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5983a-120">Authorization</span></span> | <span data-ttu-id="5983a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5983a-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5983a-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5983a-122">Request body</span></span>

<span data-ttu-id="5983a-123">В тексте запроса добавьте представление объекта [тииндикатор](../resources/tiindicator.md) в формате JSON, содержащем хотя бы один наблюдаемый объект.</span><span class="sxs-lookup"><span data-stu-id="5983a-123">In the request body, supply a JSON representation of a [tiIndicator](../resources/tiindicator.md) object containing at least one observable.</span></span>

## <a name="response"></a><span data-ttu-id="5983a-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="5983a-124">Response</span></span>

<span data-ttu-id="5983a-125">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5983a-125">If successful, this method returns `201 Created` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5983a-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="5983a-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5983a-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="5983a-127">Request</span></span>

<span data-ttu-id="5983a-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5983a-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5983a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5983a-129">Response</span></span>

<span data-ttu-id="5983a-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5983a-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="5983a-131">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5983a-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5983a-132">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5983a-132">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
