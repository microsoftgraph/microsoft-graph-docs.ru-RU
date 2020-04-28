---
title: Получение Акцесспаккажеассигнментрекуест
description: Получение свойств и связей объекта Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 285badec81e03f4dc71b3fcf479152a7ae39f484
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448455"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="a1b0d-103">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="a1b0d-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="a1b0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1b0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1b0d-105">В разделе [Управление обслуживанием Azure AD](../resources/entitlementmanagement-root.md)извлекаются свойства и связи объекта [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a1b0d-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1b0d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1b0d-106">Permissions</span></span>

<span data-ttu-id="a1b0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1b0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1b0d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1b0d-109">Permission type</span></span>                        | <span data-ttu-id="a1b0d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1b0d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a1b0d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1b0d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1b0d-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1b0d-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="a1b0d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1b0d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1b0d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-114">Not supported.</span></span> |
| <span data-ttu-id="a1b0d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1b0d-115">Application</span></span>                            | <span data-ttu-id="a1b0d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1b0d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1b0d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1b0d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1b0d-118">Optional query parameters</span></span>

<span data-ttu-id="a1b0d-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a1b0d-120">Например, чтобы получить запрошенный пакет Access, включите `$expand=accessPackage` его в запрос.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="a1b0d-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a1b0d-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1b0d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1b0d-122">Request headers</span></span>

| <span data-ttu-id="a1b0d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a1b0d-123">Name</span></span>      |<span data-ttu-id="a1b0d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a1b0d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a1b0d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1b0d-125">Authorization</span></span> | <span data-ttu-id="a1b0d-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-126">Bearer \{token\}.</span></span> <span data-ttu-id="a1b0d-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1b0d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1b0d-128">Request body</span></span>

<span data-ttu-id="a1b0d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1b0d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1b0d-130">Response</span></span>

<span data-ttu-id="a1b0d-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1b0d-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="a1b0d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1b0d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1b0d-133">Request</span></span>

<span data-ttu-id="a1b0d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1b0d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1b0d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="a1b0d-136">C#</span><span class="sxs-lookup"><span data-stu-id="a1b0d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1b0d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1b0d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1b0d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1b0d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1b0d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1b0d-139">Response</span></span>

<span data-ttu-id="a1b0d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-140">The following is an example of the response.</span></span>

> <span data-ttu-id="a1b0d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1b0d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "433dafca-5047-4614-95f7-a03510b1ded3",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "createdDateTime": "2019-10-25T22:55:11.623Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
