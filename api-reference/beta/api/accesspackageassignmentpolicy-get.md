---
title: Получение Акцесспаккажеассигнментполици
description: Получение свойств и связей объекта Акцесспаккажеаассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cebad5285d9c45c1c5bade244f83e23e6b16bd77
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331173"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="ecdd1-103">Получение Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="ecdd1-103">Get accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecdd1-104">В разделе [Управление обслуживанием Azure AD](../resources/entitlementmanagement-root.md)извлекаются свойства и связи объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ecdd1-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecdd1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecdd1-105">Permissions</span></span>

<span data-ttu-id="ecdd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecdd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ecdd1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecdd1-108">Permission type</span></span>                        | <span data-ttu-id="ecdd1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecdd1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ecdd1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecdd1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ecdd1-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecdd1-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ecdd1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecdd1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecdd1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-113">Not supported.</span></span> |
| <span data-ttu-id="ecdd1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecdd1-114">Application</span></span>                            | <span data-ttu-id="ecdd1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecdd1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecdd1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ecdd1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ecdd1-117">Optional query parameters</span></span>

<span data-ttu-id="ecdd1-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ecdd1-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ecdd1-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecdd1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecdd1-120">Request headers</span></span>

| <span data-ttu-id="ecdd1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ecdd1-121">Name</span></span>      |<span data-ttu-id="ecdd1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ecdd1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ecdd1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecdd1-123">Authorization</span></span> | <span data-ttu-id="ecdd1-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-124">Bearer \{token\}.</span></span> <span data-ttu-id="ecdd1-125">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecdd1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecdd1-126">Request body</span></span>

<span data-ttu-id="ecdd1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecdd1-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ecdd1-128">Response</span></span>

<span data-ttu-id="ecdd1-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-129">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecdd1-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ecdd1-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecdd1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecdd1-131">Request</span></span>

<span data-ttu-id="ecdd1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ecdd1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecdd1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="ecdd1-134">C#</span><span class="sxs-lookup"><span data-stu-id="ecdd1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecdd1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecdd1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecdd1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecdd1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ecdd1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecdd1-137">Response</span></span>

<span data-ttu-id="ecdd1-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ecdd1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ecdd1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "accessReviewSettings": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
