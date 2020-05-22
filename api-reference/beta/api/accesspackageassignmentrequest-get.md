---
title: Получение Акцесспаккажеассигнментрекуест
description: Получение свойств и связей объекта Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da26d23027cd77e986a40c66cb6e7acbdff08ef8
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345662"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="aaf14-103">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="aaf14-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="aaf14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaf14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaf14-105">В разделе [Управление обслуживанием Azure AD](../resources/entitlementmanagement-root.md)извлекаются свойства и связи объекта [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="aaf14-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaf14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aaf14-106">Permissions</span></span>

<span data-ttu-id="aaf14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaf14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aaf14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaf14-109">Permission type</span></span>                        | <span data-ttu-id="aaf14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaf14-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aaf14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaf14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aaf14-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="aaf14-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="aaf14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaf14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaf14-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaf14-114">Not supported.</span></span> |
| <span data-ttu-id="aaf14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaf14-115">Application</span></span>                            | <span data-ttu-id="aaf14-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaf14-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaf14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaf14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aaf14-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aaf14-118">Optional query parameters</span></span>

<span data-ttu-id="aaf14-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aaf14-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="aaf14-120">Например, чтобы получить запрошенный пакет Access, включите его `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="aaf14-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="aaf14-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="aaf14-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaf14-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaf14-122">Request headers</span></span>

| <span data-ttu-id="aaf14-123">Имя</span><span class="sxs-lookup"><span data-stu-id="aaf14-123">Name</span></span>      |<span data-ttu-id="aaf14-124">Описание</span><span class="sxs-lookup"><span data-stu-id="aaf14-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aaf14-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaf14-125">Authorization</span></span> | <span data-ttu-id="aaf14-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="aaf14-126">Bearer \{token\}.</span></span> <span data-ttu-id="aaf14-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="aaf14-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaf14-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aaf14-128">Request body</span></span>

<span data-ttu-id="aaf14-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aaf14-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaf14-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaf14-130">Response</span></span>

<span data-ttu-id="aaf14-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aaf14-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aaf14-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="aaf14-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aaf14-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaf14-133">Request</span></span>

<span data-ttu-id="aaf14-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaf14-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aaf14-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaf14-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="aaf14-136">C#</span><span class="sxs-lookup"><span data-stu-id="aaf14-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaf14-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaf14-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaf14-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaf14-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aaf14-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaf14-139">Response</span></span>

<span data-ttu-id="aaf14-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aaf14-140">The following is an example of the response.</span></span>

> <span data-ttu-id="aaf14-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aaf14-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
