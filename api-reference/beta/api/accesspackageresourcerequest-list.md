---
title: Список Акцесспаккажересаурцерекуестс
description: Получение списка объектов Акцесспаккажересаурцерекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5e320cff583c351e824d1ff472ebc5b60daa61a
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911639"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="71c1a-103">Список Акцесспаккажересаурцерекуестс</span><span class="sxs-lookup"><span data-stu-id="71c1a-103">List accessPackageResourceRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71c1a-104">Получение списка объектов [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="71c1a-104">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="71c1a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71c1a-105">Permissions</span></span>

<span data-ttu-id="71c1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71c1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71c1a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71c1a-108">Permission type</span></span>                        | <span data-ttu-id="71c1a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71c1a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="71c1a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71c1a-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="71c1a-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71c1a-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="71c1a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71c1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71c1a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c1a-113">Not supported.</span></span> |
| <span data-ttu-id="71c1a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71c1a-114">Application</span></span>                            | <span data-ttu-id="71c1a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c1a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71c1a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71c1a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71c1a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71c1a-117">Optional query parameters</span></span>

<span data-ttu-id="71c1a-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71c1a-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="71c1a-119">Например, чтобы получить сведения о том, кто запросил Добавление ресурса в каталог, включите `$expand=requestor` в запрос.</span><span class="sxs-lookup"><span data-stu-id="71c1a-119">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="71c1a-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="71c1a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="71c1a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71c1a-121">Request headers</span></span>

| <span data-ttu-id="71c1a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="71c1a-122">Name</span></span>      |<span data-ttu-id="71c1a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="71c1a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71c1a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71c1a-124">Authorization</span></span> | <span data-ttu-id="71c1a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71c1a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71c1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71c1a-127">Request body</span></span>

<span data-ttu-id="71c1a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71c1a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71c1a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="71c1a-129">Response</span></span>

<span data-ttu-id="71c1a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71c1a-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71c1a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="71c1a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71c1a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c1a-132">Request</span></span>

<span data-ttu-id="71c1a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71c1a-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="71c1a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="71c1a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="71c1a-135">C#</span><span class="sxs-lookup"><span data-stu-id="71c1a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71c1a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71c1a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="71c1a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71c1a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71c1a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c1a-138">Response</span></span>

<span data-ttu-id="71c1a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71c1a-139">The following is an example of the response.</span></span>

> <span data-ttu-id="71c1a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71c1a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
      "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
      "isValidationOnly": false,
      "justification": "String",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "requestType": "AdminAdd"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
