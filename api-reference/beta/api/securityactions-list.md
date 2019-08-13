---
title: Список Секуритяктионс
description: Получение списка объектов securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 02538a80ed8264b4e61bbeff57034d71a9cc011b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364140"
---
# <a name="list-securityactions"></a><span data-ttu-id="2d809-103">Список Секуритяктионс</span><span class="sxs-lookup"><span data-stu-id="2d809-103">List securityActions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d809-104">Получение списка объектов [securityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="2d809-104">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d809-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d809-105">Permissions</span></span>

<span data-ttu-id="2d809-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d809-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d809-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d809-108">Permission type</span></span>                        | <span data-ttu-id="2d809-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d809-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2d809-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d809-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d809-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d809-111">Not supported.</span></span> |
| <span data-ttu-id="2d809-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d809-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d809-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d809-113">Not supported.</span></span> |
| <span data-ttu-id="2d809-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d809-114">Application</span></span>                            | <span data-ttu-id="2d809-115">Секуритяктионс. Read. ALL, Секуритяктионс. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2d809-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d809-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d809-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d809-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2d809-117">Optional query parameters</span></span>

<span data-ttu-id="2d809-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2d809-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2d809-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2d809-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d809-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d809-120">Request headers</span></span>

| <span data-ttu-id="2d809-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2d809-121">Name</span></span>      |<span data-ttu-id="2d809-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2d809-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2d809-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d809-123">Authorization</span></span> | <span data-ttu-id="2d809-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2d809-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d809-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d809-125">Request body</span></span>

<span data-ttu-id="2d809-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d809-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d809-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d809-127">Response</span></span>

<span data-ttu-id="2d809-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [securityAction](../resources/securityaction.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d809-128">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d809-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d809-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d809-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d809-130">Request</span></span>

<span data-ttu-id="2d809-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d809-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2d809-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d809-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d809-133">C#</span><span class="sxs-lookup"><span data-stu-id="2d809-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityactions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d809-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d809-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityactions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d809-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2d809-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityactions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2d809-136">Java</span><span class="sxs-lookup"><span data-stu-id="2d809-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityactions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2d809-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d809-137">Response</span></span>

<span data-ttu-id="2d809-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2d809-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2d809-139">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2d809-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2d809-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d809-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "actionReason": "actionReason-value",
      "appId": "appId-value",
      "azureTenantId": "azureTenantId-value",
      "clientContext": "clientContext-value",
      "completedDateTime": "datetime-value",
      "createdDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List securityActions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
