---
title: Список Секуритяктионс
description: Получение списка объектов securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 697481d96395e5947ac3a01d29d335005bbd8dcb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044776"
---
# <a name="list-securityactions"></a><span data-ttu-id="04b3e-103">Список Секуритяктионс</span><span class="sxs-lookup"><span data-stu-id="04b3e-103">List securityActions</span></span>

<span data-ttu-id="04b3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04b3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04b3e-105">Получение списка объектов [securityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="04b3e-105">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="04b3e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04b3e-106">Permissions</span></span>

<span data-ttu-id="04b3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04b3e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04b3e-109">Permission type</span></span>                        | <span data-ttu-id="04b3e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04b3e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="04b3e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="04b3e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b3e-112">Not supported.</span></span> |
| <span data-ttu-id="04b3e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04b3e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b3e-114">Not supported.</span></span> |
| <span data-ttu-id="04b3e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04b3e-115">Application</span></span>                            | <span data-ttu-id="04b3e-116">Секуритяктионс. Read. ALL, Секуритяктионс. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="04b3e-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="04b3e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b3e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04b3e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="04b3e-118">Optional query parameters</span></span>

<span data-ttu-id="04b3e-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="04b3e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="04b3e-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="04b3e-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="04b3e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04b3e-121">Request headers</span></span>

| <span data-ttu-id="04b3e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="04b3e-122">Name</span></span>      |<span data-ttu-id="04b3e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="04b3e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="04b3e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04b3e-124">Authorization</span></span> | <span data-ttu-id="04b3e-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="04b3e-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="04b3e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04b3e-126">Request body</span></span>

<span data-ttu-id="04b3e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04b3e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04b3e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b3e-128">Response</span></span>

<span data-ttu-id="04b3e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [securityAction](../resources/securityaction.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04b3e-129">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04b3e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="04b3e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04b3e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b3e-131">Request</span></span>

<span data-ttu-id="04b3e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04b3e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04b3e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="04b3e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions
```
# <a name="c"></a>[<span data-ttu-id="04b3e-134">C#</span><span class="sxs-lookup"><span data-stu-id="04b3e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityactions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04b3e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04b3e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityactions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04b3e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04b3e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityactions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="04b3e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b3e-137">Response</span></span>

<span data-ttu-id="04b3e-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="04b3e-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="04b3e-139">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04b3e-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="04b3e-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04b3e-140">All the properties will be returned from an actual call.</span></span>

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


