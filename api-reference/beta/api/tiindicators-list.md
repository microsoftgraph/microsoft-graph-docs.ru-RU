---
title: Список индикаторов логики операций с угрозами
description: Получение списка объектов тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 98f058d94c101a2f664f21ea05252a51476b426d
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366912"
---
# <a name="list-threat-intelligence-indicators"></a><span data-ttu-id="14867-103">Список индикаторов логики операций с угрозами</span><span class="sxs-lookup"><span data-stu-id="14867-103">List threat intelligence indicators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14867-104">Получение списка объектов [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="14867-104">Retrieve a list of [tiIndicator](../resources/tiindicator.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="14867-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14867-105">Permissions</span></span>

<span data-ttu-id="14867-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14867-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14867-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14867-108">Permission type</span></span>     | <span data-ttu-id="14867-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14867-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14867-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14867-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="14867-111">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="14867-111">ThreatIndicators.ReadWrite.OwnedBy</span></span>  |
| <span data-ttu-id="14867-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14867-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14867-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14867-113">Not supported.</span></span> |
| <span data-ttu-id="14867-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14867-114">Application</span></span>                            | <span data-ttu-id="14867-115">Среатиндикаторс. ReadWrite. Овнедби</span><span class="sxs-lookup"><span data-stu-id="14867-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="14867-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14867-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14867-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="14867-117">Optional query parameters</span></span>

<span data-ttu-id="14867-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="14867-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="14867-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="14867-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="14867-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14867-120">Request headers</span></span>

| <span data-ttu-id="14867-121">Имя</span><span class="sxs-lookup"><span data-stu-id="14867-121">Name</span></span>      |<span data-ttu-id="14867-122">Описание</span><span class="sxs-lookup"><span data-stu-id="14867-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14867-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14867-123">Authorization</span></span> | <span data-ttu-id="14867-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="14867-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="14867-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14867-125">Request body</span></span>

<span data-ttu-id="14867-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14867-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14867-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="14867-127">Response</span></span>

<span data-ttu-id="14867-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [тииндикатор](../resources/tiindicator.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14867-128">If successful, this method returns a `200 OK` response code and a collection of [tiIndicator](../resources/tiindicator.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14867-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="14867-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14867-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="14867-130">Request</span></span>

<span data-ttu-id="14867-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14867-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tiindicators"
}-->

```http
GET https://graph.microsoft.com/beta/security/tiIndicators
```

### <a name="response"></a><span data-ttu-id="14867-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="14867-132">Response</span></span>

<span data-ttu-id="14867-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="14867-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="14867-134">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="14867-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="14867-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14867-135">All the properties will be returned from an actual call.</span></span>

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
      "action": "action-value",
      "activityGroupNames": [
        "activityGroupNames-value"
      ],
      "additionalInformation": "additionalInformation-value",
      "azureTenantId": "azureTenantId-value",
      "confidence": 99,
      "description": "description-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tiIndicators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
