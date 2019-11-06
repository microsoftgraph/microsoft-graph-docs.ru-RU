---
title: Список Акцесспаккажересаурцеролескопес
description: Получение списка объектов акцесспаккажересаурцеролескопе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee39c846fc40a89d28490c4ee5782a9f75b68f18
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994201"
---
# <a name="list-accesspackageresourcerolescopes"></a><span data-ttu-id="05e3b-103">Список Акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="05e3b-103">List accessPackageResourceRoleScopes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05e3b-104">Получение пакета Access со списком объектов [акцесспаккажересаурцеролескопе](../resources/accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="05e3b-104">Retrieve an access package with a list of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.</span></span>  <span data-ttu-id="05e3b-105">Каждый объект связывается с [акцесспаккажересаурцероле](../resources/accesspackageresourcerole.md) и [акцесспаккажересаурцескопе](../resources/accesspackageresourcescope.md).</span><span class="sxs-lookup"><span data-stu-id="05e3b-105">Each object links to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05e3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05e3b-106">Permissions</span></span>

<span data-ttu-id="05e3b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05e3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05e3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05e3b-109">Permission type</span></span>                        | <span data-ttu-id="05e3b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05e3b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05e3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05e3b-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="05e3b-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05e3b-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="05e3b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05e3b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05e3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05e3b-114">Not supported.</span></span> |
| <span data-ttu-id="05e3b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05e3b-115">Application</span></span>                            | <span data-ttu-id="05e3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05e3b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05e3b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05e3b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05e3b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="05e3b-118">Optional query parameters</span></span>

<span data-ttu-id="05e3b-119">Этот метод использует параметры запроса OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="05e3b-119">This method uses OData query parameters to customize the response.</span></span> <span data-ttu-id="05e3b-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="05e3b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="05e3b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05e3b-121">Request headers</span></span>

| <span data-ttu-id="05e3b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="05e3b-122">Name</span></span>      |<span data-ttu-id="05e3b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="05e3b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05e3b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="05e3b-124">Authorization</span></span> | <span data-ttu-id="05e3b-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="05e3b-125">Bearer \{token\}.</span></span> <span data-ttu-id="05e3b-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="05e3b-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05e3b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05e3b-127">Request body</span></span>

<span data-ttu-id="05e3b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05e3b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05e3b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="05e3b-129">Response</span></span>

<span data-ttu-id="05e3b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [акцесспаккаже](../resources/accesspackage.md) , содержащий коллекцию объектов [акцесспаккажересаурцеролескопе](../resources/accesspackageresourcerolescope.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05e3b-130">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) containing a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05e3b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="05e3b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05e3b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="05e3b-132">Request</span></span>

<span data-ttu-id="05e3b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05e3b-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="05e3b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="05e3b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescopes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="05e3b-135">C#</span><span class="sxs-lookup"><span data-stu-id="05e3b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerolescopes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05e3b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05e3b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerolescopes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05e3b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05e3b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerolescopes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05e3b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="05e3b-138">Response</span></span>

<span data-ttu-id="05e3b-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05e3b-139">The following is an example of the response.</span></span>

> <span data-ttu-id="05e3b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05e3b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "id": "933a4822-aed1-445b-9623-62116cd07a39",
    "catalogId": "32efb28c-9a7a-446c-986b-ca6528c6669d",
    "displayName": "Test Package 9-9",
    "description": "Test Package 9-9",
    "isHidden": false,
    "accessPackageResourceRoleScopes": [
        {
            "id": "70113acf-4dcb-453f-b517-2394598d974e_22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
            "createdBy": "alice@contoso.com",
            "createdDateTime": "2019-09-09T19:54:14.853Z",
            "modifiedBy": "alice@contoso.com",
            "modifiedDateTime": "2019-09-09T19:54:14.853Z",
            "accessPackageResourceRole": {
                "id": "70113acf-4dcb-453f-b517-2394598d974e",
                "displayName": "Owner",
                "originSystem": "origin-type",
                "originId": "Owner_7b56ede0-9b58-40bd-b11e-b3d18fc32698"
            },
            "accessPackageResourceScope": {
                "id": "22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
                "displayName": "Root",
                "description": "Root Scope",
                "originId": "7b56ede0-9b58-40bd-b11e-b3d18fc32698",
                "originSystem": "origin-type",
                "isRootScope": true
            }
        }
    ]
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoleScopes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
