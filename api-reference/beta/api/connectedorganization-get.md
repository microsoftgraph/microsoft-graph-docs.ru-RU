---
title: Получение Коннектедорганизатион
description: Получение свойств и связей объекта коннектедорганизатион.
author: markwahl-msft
ms.prod: microsoft-identity-platform
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 8df2a52ac4ad0c459c79d911bd2454f29b7bd15a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566599"
---
# <a name="get-connectedorganization"></a><span data-ttu-id="9ca06-103">Получение Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="9ca06-103">Get connectedOrganization</span></span>

<span data-ttu-id="9ca06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ca06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ca06-105">Получение свойств и связей объекта [коннектедорганизатион](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="9ca06-105">Retrieve the properties and relationships of a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ca06-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ca06-106">Permissions</span></span>

<span data-ttu-id="9ca06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ca06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ca06-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ca06-109">Permission type</span></span>|<span data-ttu-id="9ca06-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ca06-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="9ca06-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ca06-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ca06-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9ca06-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9ca06-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ca06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ca06-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ca06-114">Not supported.</span></span> |
| <span data-ttu-id="9ca06-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ca06-115">Application</span></span>                            | <span data-ttu-id="9ca06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ca06-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ca06-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ca06-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ca06-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9ca06-118">Optional query parameters</span></span>

<span data-ttu-id="9ca06-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9ca06-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9ca06-120">Например, чтобы получить только источники удостоверений, добавьте `$select=identitySources` .</span><span class="sxs-lookup"><span data-stu-id="9ca06-120">For example, to retrieve only the identity sources, add `$select=identitySources`.</span></span> <span data-ttu-id="9ca06-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9ca06-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ca06-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ca06-122">Request headers</span></span>

|<span data-ttu-id="9ca06-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9ca06-123">Name</span></span>|<span data-ttu-id="9ca06-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9ca06-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9ca06-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ca06-125">Authorization</span></span>|<span data-ttu-id="9ca06-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ca06-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ca06-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ca06-128">Request body</span></span>

<span data-ttu-id="9ca06-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ca06-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ca06-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ca06-130">Response</span></span>

<span data-ttu-id="9ca06-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коннектедорганизатион](../resources/connectedorganization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ca06-131">If successful, this method returns a `200 OK` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ca06-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ca06-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ca06-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ca06-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9ca06-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ca06-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganization"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="9ca06-135">C#</span><span class="sxs-lookup"><span data-stu-id="9ca06-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ca06-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ca06-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ca06-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ca06-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ca06-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ca06-138">Response</span></span>

<span data-ttu-id="9ca06-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ca06-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
