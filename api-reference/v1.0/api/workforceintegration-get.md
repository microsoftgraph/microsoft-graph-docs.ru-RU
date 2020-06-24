---
title: Получение Воркфорцеинтегратион
description: Получение свойств и связей объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aa08c99cdca34a9561c81e0f90ac4f61fdb15871
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845759"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="3722b-103">Получение Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="3722b-103">Get workforceIntegration</span></span>

<span data-ttu-id="3722b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3722b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3722b-105">Получение свойств и связей объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="3722b-105">Retrieve the properties and relationships of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3722b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3722b-106">Permissions</span></span>

<span data-ttu-id="3722b-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3722b-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3722b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3722b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3722b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3722b-109">Permission type</span></span>                        | <span data-ttu-id="3722b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3722b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3722b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3722b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3722b-112">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3722b-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="3722b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3722b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3722b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3722b-114">Not supported.</span></span> |
| <span data-ttu-id="3722b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3722b-115">Application</span></span>                            | <span data-ttu-id="3722b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3722b-116">Not supported.</span></span> |

> <span data-ttu-id="3722b-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3722b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3722b-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="3722b-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3722b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3722b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3722b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3722b-120">Optional query parameters</span></span>

<span data-ttu-id="3722b-121">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3722b-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3722b-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3722b-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3722b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3722b-123">Request headers</span></span>

| <span data-ttu-id="3722b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="3722b-124">Name</span></span>      |<span data-ttu-id="3722b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3722b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3722b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3722b-126">Authorization</span></span> | <span data-ttu-id="3722b-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="3722b-127">Bearer {token}.</span></span> <span data-ttu-id="3722b-128">Required.</span><span class="sxs-lookup"><span data-stu-id="3722b-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3722b-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3722b-129">Request body</span></span>

<span data-ttu-id="3722b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3722b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3722b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3722b-131">Response</span></span>

<span data-ttu-id="3722b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3722b-132">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3722b-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="3722b-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3722b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3722b-134">Request</span></span>

<span data-ttu-id="3722b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3722b-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3722b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3722b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="c"></a>[<span data-ttu-id="3722b-137">C#</span><span class="sxs-lookup"><span data-stu-id="3722b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3722b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3722b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3722b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3722b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3722b-140">Java</span><span class="sxs-lookup"><span data-stu-id="3722b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3722b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3722b-141">Response</span></span>

<span data-ttu-id="3722b-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3722b-142">The following is an example of the response.</span></span>

> <span data-ttu-id="3722b-143">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="3722b-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3722b-144">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3722b-144">All the properties will be returned from an actual call.</span></span>

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
  "supportedEntities": "shift"
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
