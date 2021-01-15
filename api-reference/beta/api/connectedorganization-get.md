---
title: Get connectedOrganization
description: Извлечение свойств и связей объекта connectedorganization.
author: markwahl-msft
ms.prod: microsoft-identity-platform
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 27b0765bf16f4fabf5057b35ad4d1b0992ba79de
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872711"
---
# <a name="get-connectedorganization"></a><span data-ttu-id="7ab58-103">Get connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="7ab58-103">Get connectedOrganization</span></span>

<span data-ttu-id="7ab58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ab58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ab58-105">Извлечение свойств и связей объекта [connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="7ab58-105">Retrieve the properties and relationships of a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ab58-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ab58-106">Permissions</span></span>

<span data-ttu-id="7ab58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ab58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ab58-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ab58-109">Permission type</span></span>|<span data-ttu-id="7ab58-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ab58-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="7ab58-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ab58-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ab58-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ab58-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7ab58-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ab58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ab58-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ab58-114">Not supported.</span></span> |
| <span data-ttu-id="7ab58-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ab58-115">Application</span></span>                            | <span data-ttu-id="7ab58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ab58-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ab58-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ab58-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ab58-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ab58-118">Optional query parameters</span></span>

<span data-ttu-id="7ab58-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7ab58-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7ab58-120">Например, чтобы получить только источники удостоверений, добавьте `$select=identitySources` .</span><span class="sxs-lookup"><span data-stu-id="7ab58-120">For example, to retrieve only the identity sources, add `$select=identitySources`.</span></span> <span data-ttu-id="7ab58-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7ab58-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ab58-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ab58-122">Request headers</span></span>

|<span data-ttu-id="7ab58-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7ab58-123">Name</span></span>|<span data-ttu-id="7ab58-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7ab58-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7ab58-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ab58-125">Authorization</span></span>|<span data-ttu-id="7ab58-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ab58-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ab58-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ab58-128">Request body</span></span>

<span data-ttu-id="7ab58-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ab58-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ab58-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ab58-130">Response</span></span>

<span data-ttu-id="7ab58-131">В случае успеха этот метод возвращает код `200 OK` отклика и [объект connectedOrganization](../resources/connectedorganization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ab58-131">If successful, this method returns a `200 OK` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ab58-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7ab58-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ab58-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ab58-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ab58-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ab58-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganization"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="7ab58-135">C#</span><span class="sxs-lookup"><span data-stu-id="7ab58-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ab58-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ab58-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ab58-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ab58-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ab58-138">Java</span><span class="sxs-lookup"><span data-stu-id="7ab58-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7ab58-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ab58-139">Response</span></span>

<span data-ttu-id="7ab58-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7ab58-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f",
  "displayName": "Wingtip Toys",
  "description": "Wingtip Toys",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-05-13T15:18:04.81Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-05-13T15:18:04.81Z",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "bf85dc9d-cb43-44a4-80c4-469e8c58249e",
      "displayName": "Wingtip Toys Co"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


