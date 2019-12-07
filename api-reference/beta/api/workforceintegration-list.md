---
title: Список Воркфорцеинтегратионс
description: Получение списка объектов Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8081305d23f31803691cdcb6d1c39d93080113c9
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895807"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="b0dc9-103">Список Воркфорцеинтегратионс</span><span class="sxs-lookup"><span data-stu-id="b0dc9-103">List workforceIntegrations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0dc9-104">Получение списка объектов [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0dc9-104">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0dc9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0dc9-105">Permissions</span></span>

<span data-ttu-id="b0dc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0dc9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0dc9-108">Permission type</span></span>                        | <span data-ttu-id="b0dc9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0dc9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b0dc9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0dc9-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="b0dc9-111">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b0dc9-111">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="b0dc9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0dc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0dc9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-113">Not supported.</span></span> |
| <span data-ttu-id="b0dc9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0dc9-114">Application</span></span>                            | <span data-ttu-id="b0dc9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0dc9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0dc9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0dc9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0dc9-117">Optional query parameters</span></span>

<span data-ttu-id="b0dc9-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b0dc9-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b0dc9-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0dc9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0dc9-120">Request headers</span></span>

| <span data-ttu-id="b0dc9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b0dc9-121">Name</span></span>      |<span data-ttu-id="b0dc9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b0dc9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0dc9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0dc9-123">Authorization</span></span> | <span data-ttu-id="b0dc9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0dc9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0dc9-126">Request body</span></span>

<span data-ttu-id="b0dc9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0dc9-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0dc9-128">Response</span></span>

<span data-ttu-id="b0dc9-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-129">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0dc9-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0dc9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0dc9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0dc9-131">Request</span></span>

<span data-ttu-id="b0dc9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```http
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```

### <a name="response"></a><span data-ttu-id="b0dc9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0dc9-133">Response</span></span>

<span data-ttu-id="b0dc9-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-134">The following is an example of the response.</span></span>

> <span data-ttu-id="b0dc9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0dc9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "apiVersion": 99,
      "encryption": {
        "protocol": "protocol-value",
        "secret": "secret-value"
      },
      "isActive": true,
      "url": "url-value",
      "supports": "supports-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
