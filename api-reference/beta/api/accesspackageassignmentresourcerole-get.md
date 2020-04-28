---
title: Получение Акцесспаккажеассигнментресаурцероле
description: Получение свойств и связей объекта Акцесспаккажеассигнментресаурцероле.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ae44a167d7e89ac659e816e5ebe90d1995b5258b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442010"
---
# <a name="get-accesspackageassignmentresourcerole"></a><span data-ttu-id="76232-103">Получение Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="76232-103">Get accessPackageAssignmentResourceRole</span></span>

<span data-ttu-id="76232-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76232-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76232-105">Получение свойств и связей объекта [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="76232-105">Retrieve the properties and relationships of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="76232-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76232-106">Permissions</span></span>

<span data-ttu-id="76232-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76232-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76232-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76232-109">Permission type</span></span>                        | <span data-ttu-id="76232-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76232-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76232-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76232-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="76232-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76232-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="76232-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76232-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76232-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76232-114">Not supported.</span></span> |
| <span data-ttu-id="76232-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76232-115">Application</span></span>                            | <span data-ttu-id="76232-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76232-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76232-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76232-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76232-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="76232-118">Optional query parameters</span></span>

<span data-ttu-id="76232-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="76232-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="76232-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="76232-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="76232-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76232-121">Request headers</span></span>

| <span data-ttu-id="76232-122">Имя</span><span class="sxs-lookup"><span data-stu-id="76232-122">Name</span></span>      |<span data-ttu-id="76232-123">Описание</span><span class="sxs-lookup"><span data-stu-id="76232-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76232-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76232-124">Authorization</span></span> | <span data-ttu-id="76232-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76232-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76232-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76232-127">Request body</span></span>

<span data-ttu-id="76232-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76232-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76232-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="76232-129">Response</span></span>

<span data-ttu-id="76232-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76232-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76232-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="76232-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76232-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="76232-132">Request</span></span>

<span data-ttu-id="76232-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76232-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="76232-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="76232-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourcerole"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="76232-135">C#</span><span class="sxs-lookup"><span data-stu-id="76232-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourcerole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76232-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76232-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourcerole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76232-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76232-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourcerole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76232-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="76232-138">Response</span></span>

<span data-ttu-id="76232-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="76232-139">The following is an example of the response.</span></span>

> <span data-ttu-id="76232-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76232-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
