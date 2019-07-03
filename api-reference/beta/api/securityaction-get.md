---
title: Получение объекта securityAction
description: Получение свойств и связей объекта securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 6b56f6a75b5def8c3b59a8c9898c59576de5586c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457361"
---
# <a name="get-securityaction"></a><span data-ttu-id="82dbf-103">Получение объекта securityAction</span><span class="sxs-lookup"><span data-stu-id="82dbf-103">Get securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82dbf-104">Получение свойств и связей объекта [securityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="82dbf-104">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="82dbf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82dbf-105">Permissions</span></span>

<span data-ttu-id="82dbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82dbf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82dbf-108">Permission type</span></span>                        | <span data-ttu-id="82dbf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82dbf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82dbf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82dbf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="82dbf-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82dbf-111">Not supported.</span></span> |
| <span data-ttu-id="82dbf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82dbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82dbf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82dbf-113">Not supported.</span></span> |
| <span data-ttu-id="82dbf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82dbf-114">Application</span></span>                            | <span data-ttu-id="82dbf-115">Секуритяктионс. Read. ALL, Секуритяктионс. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="82dbf-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82dbf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82dbf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82dbf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82dbf-117">Optional query parameters</span></span>

<span data-ttu-id="82dbf-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="82dbf-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="82dbf-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="82dbf-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="82dbf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82dbf-120">Request headers</span></span>

| <span data-ttu-id="82dbf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="82dbf-121">Name</span></span>      |<span data-ttu-id="82dbf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="82dbf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82dbf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82dbf-123">Authorization</span></span> | <span data-ttu-id="82dbf-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="82dbf-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="82dbf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82dbf-125">Request body</span></span>

<span data-ttu-id="82dbf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82dbf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82dbf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="82dbf-127">Response</span></span>

<span data-ttu-id="82dbf-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [securityAction](../resources/securityaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82dbf-128">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82dbf-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="82dbf-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82dbf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="82dbf-130">Request</span></span>

<span data-ttu-id="82dbf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82dbf-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="82dbf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="82dbf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82dbf-133">C#</span><span class="sxs-lookup"><span data-stu-id="82dbf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82dbf-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="82dbf-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82dbf-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82dbf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82dbf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="82dbf-136">Response</span></span>

<span data-ttu-id="82dbf-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="82dbf-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="82dbf-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="82dbf-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="82dbf-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82dbf-139">All the properties will be returned from an actual call.</span></span>

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
