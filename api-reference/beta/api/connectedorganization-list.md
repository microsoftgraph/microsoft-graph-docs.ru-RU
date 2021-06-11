---
title: Списки подключенныхОрганизацией
description: Извлечение списка объектов connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d891343bdc08b29db6a8680d84bb6f12e70b23ea
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896300"
---
# <a name="list-connectedorganizations"></a><span data-ttu-id="1a911-103">Списки подключенныхОрганизацией</span><span class="sxs-lookup"><span data-stu-id="1a911-103">List connectedOrganizations</span></span>

<span data-ttu-id="1a911-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a911-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a911-105">Извлечение списка [объектов connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="1a911-105">Retrieve a list of [connectedOrganization](../resources/connectedorganization.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a911-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a911-106">Permissions</span></span>

<span data-ttu-id="1a911-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a911-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a911-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a911-109">Permission type</span></span>|<span data-ttu-id="1a911-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a911-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="1a911-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a911-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a911-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a911-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1a911-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a911-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a911-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a911-114">Not supported.</span></span> |
| <span data-ttu-id="1a911-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1a911-115">Application</span></span>                            | <span data-ttu-id="1a911-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a911-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a911-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a911-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a911-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a911-118">Optional query parameters</span></span>
<span data-ttu-id="1a911-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1a911-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1a911-120">Например, чтобы получить только подключенные организации с определенным именем отображения, добавьте `$filter=displayName eq 'Name'` .</span><span class="sxs-lookup"><span data-stu-id="1a911-120">For example, to retrieve only the connected organizations with a specific display name, add `$filter=displayName eq 'Name'`.</span></span> <span data-ttu-id="1a911-121">Аналогичным образом, чтобы получить только подключенные организации с источником удостоверений определенного клиента, добавьте `$filter=identitySources/any(is:is/microsoft.graph.azureActiveDirectoryTenant/tenantId eq '72f988bf-86f1-41af-91ab-2d7cd011db47')` .</span><span class="sxs-lookup"><span data-stu-id="1a911-121">Similarly, to retrieve only the connected organizations with an identity source of a specific tenant, add `$filter=identitySources/any(is:is/microsoft.graph.azureActiveDirectoryTenant/tenantId eq '72f988bf-86f1-41af-91ab-2d7cd011db47')`.</span></span> <span data-ttu-id="1a911-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1a911-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a911-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a911-123">Request headers</span></span>
|<span data-ttu-id="1a911-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1a911-124">Name</span></span>|<span data-ttu-id="1a911-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1a911-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1a911-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a911-126">Authorization</span></span>|<span data-ttu-id="1a911-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a911-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a911-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a911-129">Request body</span></span>
<span data-ttu-id="1a911-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a911-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a911-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a911-131">Response</span></span>

<span data-ttu-id="1a911-132">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов connectedOrganization](../resources/connectedorganization.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1a911-132">If successful, this method returns a `200 OK` response code and a collection of [connectedOrganization](../resources/connectedorganization.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a911-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a911-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a911-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a911-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1a911-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a911-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganizations"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations
```
# <a name="c"></a>[<span data-ttu-id="1a911-136">C#</span><span class="sxs-lookup"><span data-stu-id="1a911-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a911-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a911-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a911-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a911-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a911-139">Java</span><span class="sxs-lookup"><span data-stu-id="1a911-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a911-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a911-140">Response</span></span>
<span data-ttu-id="1a911-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1a911-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.connectedOrganization)"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectedOrganizations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


