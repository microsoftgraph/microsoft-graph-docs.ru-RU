---
title: Получение Акцесспаккажеассигнментресаурцероле
description: Получение свойств и связей объекта Акцесспаккажеассигнментресаурцероле.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 18f6cfedbd0ddc116d6d4214c9cfbb12184009e5
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345648"
---
# <a name="get-accesspackageassignmentresourcerole"></a><span data-ttu-id="964a6-103">Получение Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="964a6-103">Get accessPackageAssignmentResourceRole</span></span>

<span data-ttu-id="964a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="964a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="964a6-105">Получение свойств и связей объекта [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="964a6-105">Retrieve the properties and relationships of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="964a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="964a6-106">Permissions</span></span>

<span data-ttu-id="964a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="964a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="964a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="964a6-109">Permission type</span></span>                        | <span data-ttu-id="964a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="964a6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="964a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="964a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="964a6-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="964a6-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="964a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="964a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="964a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="964a6-114">Not supported.</span></span> |
| <span data-ttu-id="964a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="964a6-115">Application</span></span>                            | <span data-ttu-id="964a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="964a6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="964a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="964a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="964a6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="964a6-118">Optional query parameters</span></span>

<span data-ttu-id="964a6-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="964a6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="964a6-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="964a6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="964a6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="964a6-121">Request headers</span></span>

| <span data-ttu-id="964a6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="964a6-122">Name</span></span>      |<span data-ttu-id="964a6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="964a6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="964a6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="964a6-124">Authorization</span></span> | <span data-ttu-id="964a6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="964a6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="964a6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="964a6-127">Request body</span></span>

<span data-ttu-id="964a6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="964a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="964a6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="964a6-129">Response</span></span>

<span data-ttu-id="964a6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="964a6-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="964a6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="964a6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="964a6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="964a6-132">Request</span></span>

<span data-ttu-id="964a6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="964a6-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="964a6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="964a6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourcerole"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="964a6-135">C#</span><span class="sxs-lookup"><span data-stu-id="964a6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourcerole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="964a6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="964a6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourcerole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="964a6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="964a6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourcerole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="964a6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="964a6-138">Response</span></span>

<span data-ttu-id="964a6-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="964a6-139">The following is an example of the response.</span></span>

> <span data-ttu-id="964a6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="964a6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
  "originId": "originId-value",
  "originSystem": "SharePointOnline",
  "status": "Fulfilled"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentResourceRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
