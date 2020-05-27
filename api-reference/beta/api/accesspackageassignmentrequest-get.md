---
title: Получение Акцесспаккажеассигнментрекуест
description: Получение свойств и связей объекта Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f218e01cf389668ea1f7b680c2c58af4afa9094
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383499"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="50710-103">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="50710-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="50710-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50710-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50710-105">В разделе [Управление обслуживанием Azure AD](../resources/entitlementmanagement-root.md)извлекаются свойства и связи объекта [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="50710-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="50710-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50710-106">Permissions</span></span>

<span data-ttu-id="50710-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50710-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50710-109">Permission type</span></span>                        | <span data-ttu-id="50710-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50710-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="50710-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50710-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="50710-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="50710-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="50710-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50710-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50710-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50710-114">Not supported.</span></span> |
| <span data-ttu-id="50710-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50710-115">Application</span></span>                            | <span data-ttu-id="50710-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50710-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50710-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50710-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50710-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50710-118">Optional query parameters</span></span>

<span data-ttu-id="50710-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50710-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="50710-120">Например, чтобы получить запрошенный пакет Access, включите его `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="50710-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="50710-121">Чтобы получить результирующее назначение, включите `$expand=accessPackageAssignment` в запрос.</span><span class="sxs-lookup"><span data-stu-id="50710-121">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="50710-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="50710-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="50710-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50710-123">Request headers</span></span>

| <span data-ttu-id="50710-124">Имя</span><span class="sxs-lookup"><span data-stu-id="50710-124">Name</span></span>      |<span data-ttu-id="50710-125">Описание</span><span class="sxs-lookup"><span data-stu-id="50710-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50710-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="50710-126">Authorization</span></span> | <span data-ttu-id="50710-127">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="50710-127">Bearer \{token\}.</span></span> <span data-ttu-id="50710-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="50710-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50710-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50710-129">Request body</span></span>

<span data-ttu-id="50710-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50710-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50710-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="50710-131">Response</span></span>

<span data-ttu-id="50710-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50710-132">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="50710-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="50710-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50710-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="50710-134">Request</span></span>

<span data-ttu-id="50710-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50710-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50710-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="50710-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="50710-137">C#</span><span class="sxs-lookup"><span data-stu-id="50710-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50710-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50710-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50710-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50710-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50710-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="50710-140">Response</span></span>

<span data-ttu-id="50710-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="50710-141">The following is an example of the response.</span></span>

> <span data-ttu-id="50710-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50710-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
