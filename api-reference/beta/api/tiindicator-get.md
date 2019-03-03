---
title: Получение индикатора логики операций с угрозами
description: Получение свойств и связей объекта тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5376200bc2824d51dd1eec2a442b797836855fdb
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366926"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="c2624-103">Получение индикатора логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="c2624-103">Get threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2624-104">Получение свойств и связей объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="c2624-104">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2624-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2624-105">Permissions</span></span>

<span data-ttu-id="c2624-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2624-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2624-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2624-108">Permission type</span></span>                        | <span data-ttu-id="c2624-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2624-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c2624-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2624-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2624-111">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="c2624-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="c2624-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2624-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2624-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2624-113">Not supported.</span></span> |
| <span data-ttu-id="c2624-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2624-114">Application</span></span>                            | <span data-ttu-id="c2624-115">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="c2624-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2624-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2624-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2624-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2624-117">Optional query parameters</span></span>

<span data-ttu-id="c2624-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2624-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c2624-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c2624-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2624-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2624-120">Request headers</span></span>

| <span data-ttu-id="c2624-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c2624-121">Name</span></span>      |<span data-ttu-id="c2624-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c2624-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2624-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2624-123">Authorization</span></span> | <span data-ttu-id="c2624-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c2624-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2624-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2624-125">Request body</span></span>

<span data-ttu-id="c2624-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2624-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2624-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2624-127">Response</span></span>

<span data-ttu-id="c2624-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2624-128">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2624-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c2624-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2624-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2624-130">Request</span></span>

<span data-ttu-id="c2624-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2624-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="c2624-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2624-132">Response</span></span>

<span data-ttu-id="c2624-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2624-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c2624-134">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2624-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c2624-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2624-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "action": "action-value",
  "activityGroupNames": [
    "activityGroupNames-value"
  ],
  "additionalInformation": "additionalInformation-value",
  "azureTenantId": "azureTenantId-value",
  "confidence": 99,
  "description": "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
