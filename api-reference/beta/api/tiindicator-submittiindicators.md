---
title: 'Тииндикатор: Субмиттииндикаторс'
description: Отправьте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b6d3e530fc571029c3b71675ca195e7bb046c823
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366975"
---
# <a name="tiindicator-submittiindicators"></a><span data-ttu-id="24521-103">Тииндикатор: Субмиттииндикаторс</span><span class="sxs-lookup"><span data-stu-id="24521-103">tiIndicator: submitTiIndicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24521-104">Отправьте несколько индикаторов системы анализа угроз (TI) в одном запросе, а не нескольких запросах.</span><span class="sxs-lookup"><span data-stu-id="24521-104">Upload multiple threat intelligence (TI) indicators in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="24521-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24521-105">Permissions</span></span>

<span data-ttu-id="24521-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24521-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24521-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24521-108">Permission type</span></span> | <span data-ttu-id="24521-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24521-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="24521-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24521-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="24521-111">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="24521-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="24521-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24521-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24521-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24521-113">Not supported.</span></span> |
| <span data-ttu-id="24521-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24521-114">Application</span></span>                            | <span data-ttu-id="24521-115">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="24521-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="24521-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24521-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/tiIndicators/submitTiIndicators
```

## <a name="request-headers"></a><span data-ttu-id="24521-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24521-117">Request headers</span></span>

| <span data-ttu-id="24521-118">Имя</span><span class="sxs-lookup"><span data-stu-id="24521-118">Name</span></span>          | <span data-ttu-id="24521-119">Описание</span><span class="sxs-lookup"><span data-stu-id="24521-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="24521-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24521-120">Authorization</span></span> | <span data-ttu-id="24521-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="24521-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="24521-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24521-122">Request body</span></span>

<span data-ttu-id="24521-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="24521-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24521-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="24521-124">Parameter</span></span>    | <span data-ttu-id="24521-125">Тип</span><span class="sxs-lookup"><span data-stu-id="24521-125">Type</span></span>        | <span data-ttu-id="24521-126">Описание</span><span class="sxs-lookup"><span data-stu-id="24521-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="24521-127">value</span><span class="sxs-lookup"><span data-stu-id="24521-127">value</span></span>|<span data-ttu-id="24521-128">Коллекция Тииндикатор</span><span class="sxs-lookup"><span data-stu-id="24521-128">tiIndicator collection</span></span>| <span data-ttu-id="24521-129">Коллекция объектов **тииндикаторс** , которую необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="24521-129">JSON collection of **tiIndicators** to be created.</span></span> |

## <a name="response"></a><span data-ttu-id="24521-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="24521-130">Response</span></span>

<span data-ttu-id="24521-131">В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24521-131">If successful, this method returns `200, OK` response code and a [tiIndicator](../resources/tiindicator.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24521-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="24521-132">Examples</span></span>

<span data-ttu-id="24521-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="24521-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="24521-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="24521-134">Request</span></span>

<span data-ttu-id="24521-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24521-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tiindicator_submittiindicators"
}-->

```http
POST https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators
Content-type: application/json

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

### <a name="response"></a><span data-ttu-id="24521-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="24521-136">Response</span></span>

<span data-ttu-id="24521-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="24521-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="24521-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="24521-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="24521-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24521-139">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
