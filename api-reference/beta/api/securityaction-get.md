---
title: Получение объекта securityAction
description: Извлечение свойств и связей объекта securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 328a54bb73517611b3fc96603601309cbb1a7ea7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050873"
---
# <a name="get-securityaction"></a><span data-ttu-id="2ff8c-103">Получение объекта securityAction</span><span class="sxs-lookup"><span data-stu-id="2ff8c-103">Get securityAction</span></span>

<span data-ttu-id="2ff8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ff8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ff8c-105">Извлечение свойств и связей объекта [securityAction.](../resources/securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="2ff8c-105">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ff8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ff8c-106">Permissions</span></span>

<span data-ttu-id="2ff8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ff8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ff8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ff8c-109">Permission type</span></span>                        | <span data-ttu-id="2ff8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ff8c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ff8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ff8c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ff8c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ff8c-112">Not supported.</span></span> |
| <span data-ttu-id="2ff8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ff8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ff8c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ff8c-114">Not supported.</span></span> |
| <span data-ttu-id="2ff8c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2ff8c-115">Application</span></span>                            | <span data-ttu-id="2ff8c-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ff8c-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ff8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ff8c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ff8c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2ff8c-118">Optional query parameters</span></span>

<span data-ttu-id="2ff8c-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2ff8c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ff8c-120">Общие сведения см. в [окне Параметры запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="2ff8c-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ff8c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ff8c-121">Request headers</span></span>

| <span data-ttu-id="2ff8c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2ff8c-122">Name</span></span>      |<span data-ttu-id="2ff8c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff8c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ff8c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ff8c-124">Authorization</span></span> | <span data-ttu-id="2ff8c-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2ff8c-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ff8c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ff8c-126">Request body</span></span>

<span data-ttu-id="2ff8c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ff8c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ff8c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ff8c-128">Response</span></span>

<span data-ttu-id="2ff8c-129">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [securityAction](../resources/securityaction.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2ff8c-129">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ff8c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ff8c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ff8c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ff8c-131">Request</span></span>

<span data-ttu-id="2ff8c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ff8c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ff8c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ff8c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```
# <a name="c"></a>[<span data-ttu-id="2ff8c-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ff8c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ff8c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ff8c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ff8c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ff8c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ff8c-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ff8c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ff8c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ff8c-138">Response</span></span>

<span data-ttu-id="2ff8c-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ff8c-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2ff8c-140">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ff8c-140">The response object shown here might be shortened for readability.</span></span>

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


