---
title: Получение объекта securityAction
description: Получение свойств и связей объекта securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 4bb2829845db6b5cf5134ff6aecec7708ff0fa81
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976442"
---
# <a name="get-securityaction"></a><span data-ttu-id="1dc61-103">Получение объекта securityAction</span><span class="sxs-lookup"><span data-stu-id="1dc61-103">Get securityAction</span></span>

<span data-ttu-id="1dc61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dc61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dc61-105">Получение свойств и связей объекта [securityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="1dc61-105">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dc61-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dc61-106">Permissions</span></span>

<span data-ttu-id="1dc61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dc61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1dc61-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dc61-109">Permission type</span></span>                        | <span data-ttu-id="1dc61-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dc61-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1dc61-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dc61-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dc61-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dc61-112">Not supported.</span></span> |
| <span data-ttu-id="1dc61-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dc61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dc61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dc61-114">Not supported.</span></span> |
| <span data-ttu-id="1dc61-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1dc61-115">Application</span></span>                            | <span data-ttu-id="1dc61-116">Секуритяктионс. Read. ALL, Секуритяктионс. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1dc61-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dc61-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dc61-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1dc61-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1dc61-118">Optional query parameters</span></span>

<span data-ttu-id="1dc61-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1dc61-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1dc61-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1dc61-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dc61-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dc61-121">Request headers</span></span>

| <span data-ttu-id="1dc61-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1dc61-122">Name</span></span>      |<span data-ttu-id="1dc61-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1dc61-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1dc61-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dc61-124">Authorization</span></span> | <span data-ttu-id="1dc61-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1dc61-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dc61-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1dc61-126">Request body</span></span>

<span data-ttu-id="1dc61-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dc61-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dc61-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dc61-128">Response</span></span>

<span data-ttu-id="1dc61-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [securityAction](../resources/securityaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1dc61-129">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1dc61-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="1dc61-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1dc61-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dc61-131">Request</span></span>

<span data-ttu-id="1dc61-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dc61-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1dc61-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dc61-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```
# <a name="c"></a>[<span data-ttu-id="1dc61-134">C#</span><span class="sxs-lookup"><span data-stu-id="1dc61-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dc61-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dc61-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dc61-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dc61-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dc61-137">Java</span><span class="sxs-lookup"><span data-stu-id="1dc61-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1dc61-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dc61-138">Response</span></span>

<span data-ttu-id="1dc61-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1dc61-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1dc61-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1dc61-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1dc61-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dc61-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


