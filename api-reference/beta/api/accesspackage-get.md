---
title: Получение Акцесспаккаже
description: Получение свойств и связей объекта Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1278c352cb69b5a25c64437a554911866f23294b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448559"
---
# <a name="get-accesspackage"></a><span data-ttu-id="0278c-103">Получение Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="0278c-103">Get accessPackage</span></span>

<span data-ttu-id="0278c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0278c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0278c-105">Получение свойств и связей объекта [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="0278c-105">Retrieve the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0278c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0278c-106">Permissions</span></span>

<span data-ttu-id="0278c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0278c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0278c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0278c-109">Permission type</span></span>                        | <span data-ttu-id="0278c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0278c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0278c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0278c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0278c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0278c-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="0278c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0278c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0278c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0278c-114">Not supported.</span></span> |
| <span data-ttu-id="0278c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0278c-115">Application</span></span>                            | <span data-ttu-id="0278c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0278c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0278c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0278c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0278c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0278c-118">Optional query parameters</span></span>

<span data-ttu-id="0278c-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0278c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0278c-120">Например, чтобы получить доступ к политикам пакетов доступа, `$expand=accessPackageAssignmentPolicies`добавьте.</span><span class="sxs-lookup"><span data-stu-id="0278c-120">For example, to retrieve the access package policies, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="0278c-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0278c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0278c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0278c-122">Request headers</span></span>

| <span data-ttu-id="0278c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0278c-123">Name</span></span>      |<span data-ttu-id="0278c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0278c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0278c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0278c-125">Authorization</span></span> | <span data-ttu-id="0278c-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="0278c-126">Bearer \{token\}.</span></span> <span data-ttu-id="0278c-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="0278c-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0278c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0278c-128">Request body</span></span>

<span data-ttu-id="0278c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0278c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0278c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0278c-130">Response</span></span>

<span data-ttu-id="0278c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккаже](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0278c-131">If successful, this method returns a `200 OK` response code and the requested [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0278c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="0278c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0278c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0278c-133">Request</span></span>

<span data-ttu-id="0278c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0278c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0278c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0278c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="0278c-136">C#</span><span class="sxs-lookup"><span data-stu-id="0278c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0278c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0278c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0278c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0278c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0278c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0278c-139">Response</span></span>

<span data-ttu-id="0278c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0278c-140">The following is an example of the response.</span></span>

> <span data-ttu-id="0278c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0278c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
