---
title: Получение Воркфорцеинтегратион
description: Получение свойств и связей объекта воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2738959b356faba1d6d27ae48fa94dcf6f28dbe9
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895803"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="e6888-103">Получение Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="e6888-103">Get workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6888-104">Получение свойств и связей объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="e6888-104">Retrieve the properties and relationships of [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6888-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6888-105">Permissions</span></span>

<span data-ttu-id="e6888-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6888-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6888-108">Permission type</span></span>                        | <span data-ttu-id="e6888-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6888-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e6888-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6888-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6888-111">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e6888-111">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="e6888-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6888-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6888-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6888-113">Not supported.</span></span> |
| <span data-ttu-id="e6888-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6888-114">Application</span></span>                            | <span data-ttu-id="e6888-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6888-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6888-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6888-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e6888-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6888-117">Optional query parameters</span></span>

<span data-ttu-id="e6888-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6888-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e6888-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e6888-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6888-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6888-120">Request headers</span></span>

| <span data-ttu-id="e6888-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e6888-121">Name</span></span>      |<span data-ttu-id="e6888-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e6888-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6888-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6888-123">Authorization</span></span> | <span data-ttu-id="e6888-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e6888-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6888-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6888-125">Request body</span></span>

<span data-ttu-id="e6888-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6888-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6888-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6888-127">Response</span></span>

<span data-ttu-id="e6888-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6888-128">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6888-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="e6888-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6888-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6888-130">Request</span></span>

<span data-ttu-id="e6888-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6888-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```http
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceintegrationid}
```

### <a name="response"></a><span data-ttu-id="e6888-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6888-132">Response</span></span>

<span data-ttu-id="e6888-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e6888-133">The following is an example of the response.</span></span>

> <span data-ttu-id="e6888-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6888-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supports": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->