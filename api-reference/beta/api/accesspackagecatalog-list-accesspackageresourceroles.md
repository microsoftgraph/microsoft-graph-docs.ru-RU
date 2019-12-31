---
title: Список Акцесспаккажересаурцеролес
description: Получение списка объектов Акцесспаккажересаурцероле.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 435f093173e112324e02987826b42b17a8c18138
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911660"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="1f5f5-103">Список Акцесспаккажересаурцеролес</span><span class="sxs-lookup"><span data-stu-id="1f5f5-103">List accessPackageResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f5f5-104">Получение списка объектов [акцесспаккажересаурцероле](../resources/accesspackageresourcerole.md) объекта [акцесспаккажересаурце](../resources/accesspackageresource.md) в [акцесспаккажекаталог](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="1f5f5-104">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="1f5f5-105">Этот список ролей затем может использоваться вызывающим абонентом для выбора роли, которая необходима при последующем [создании акцесспаккажересаурцеролескопе](accesspackage-post-accesspackageresourcerolescopes.md).</span><span class="sxs-lookup"><span data-stu-id="1f5f5-105">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f5f5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f5f5-106">Permissions</span></span>

<span data-ttu-id="1f5f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f5f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f5f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f5f5-109">Permission type</span></span>                        | <span data-ttu-id="1f5f5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f5f5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f5f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f5f5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f5f5-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f5f5-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1f5f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f5f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f5f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-114">Not supported.</span></span> |
| <span data-ttu-id="1f5f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f5f5-115">Application</span></span>                            | <span data-ttu-id="1f5f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f5f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f5f5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f5f5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f5f5-118">Optional query parameters</span></span>

<span data-ttu-id="1f5f5-119">Этот метод использует параметры запроса OData для создания отклика.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-119">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="1f5f5-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1f5f5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f5f5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f5f5-121">Request headers</span></span>

| <span data-ttu-id="1f5f5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1f5f5-122">Name</span></span>      |<span data-ttu-id="1f5f5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1f5f5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f5f5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f5f5-124">Authorization</span></span> | <span data-ttu-id="1f5f5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f5f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f5f5-127">Request body</span></span>

<span data-ttu-id="1f5f5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f5f5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f5f5-129">Response</span></span>

<span data-ttu-id="1f5f5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажересаурцероле](../resources/accesspackageresourcerole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f5f5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1f5f5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f5f5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f5f5-132">Request</span></span>

<span data-ttu-id="1f5f5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1f5f5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f5f5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1f5f5-135">C#</span><span class="sxs-lookup"><span data-stu-id="1f5f5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f5f5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f5f5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1f5f5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f5f5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f5f5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f5f5-138">Response</span></span>

<span data-ttu-id="1f5f5-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-139">The following is an example of the response.</span></span>

> <span data-ttu-id="1f5f5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f5f5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "displayName": "Member",
      "description": "description-value",
      "originId": "originId-value",
      "originSystem": "originSystem-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
