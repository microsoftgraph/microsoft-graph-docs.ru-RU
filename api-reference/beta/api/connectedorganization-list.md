---
title: Список Коннектедорганизатионс
description: Получение списка объектов Коннектедорганизатион.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5e11c6eac2be1358faa3b22ad388bcd360ad51bc
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566580"
---
# <a name="list-connectedorganizations"></a><span data-ttu-id="917f7-103">Список Коннектедорганизатионс</span><span class="sxs-lookup"><span data-stu-id="917f7-103">List connectedOrganizations</span></span>

<span data-ttu-id="917f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="917f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="917f7-105">Получение списка объектов [коннектедорганизатион](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="917f7-105">Retrieve a list of [connectedOrganization](../resources/connectedorganization.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="917f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="917f7-106">Permissions</span></span>

<span data-ttu-id="917f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="917f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="917f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="917f7-109">Permission type</span></span>|<span data-ttu-id="917f7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="917f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="917f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="917f7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="917f7-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="917f7-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="917f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="917f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="917f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="917f7-114">Not supported.</span></span> |
| <span data-ttu-id="917f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="917f7-115">Application</span></span>                            | <span data-ttu-id="917f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="917f7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="917f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="917f7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="917f7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="917f7-118">Optional query parameters</span></span>
<span data-ttu-id="917f7-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="917f7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="917f7-120">Например, чтобы получить только подключенные Организации с определенным отображаемым именем, добавьте `$filter=displayName eq 'Name'` .</span><span class="sxs-lookup"><span data-stu-id="917f7-120">For example, to retrieve only the connected organizations with a specific display name, add `$filter=displayName eq 'Name'`.</span></span> <span data-ttu-id="917f7-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="917f7-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="917f7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="917f7-122">Request headers</span></span>
|<span data-ttu-id="917f7-123">Имя</span><span class="sxs-lookup"><span data-stu-id="917f7-123">Name</span></span>|<span data-ttu-id="917f7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="917f7-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="917f7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="917f7-125">Authorization</span></span>|<span data-ttu-id="917f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="917f7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="917f7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="917f7-128">Request body</span></span>
<span data-ttu-id="917f7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="917f7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="917f7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="917f7-130">Response</span></span>

<span data-ttu-id="917f7-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [коннектедорганизатион](../resources/connectedorganization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="917f7-131">If successful, this method returns a `200 OK` response code and a collection of [connectedOrganization](../resources/connectedorganization.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="917f7-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="917f7-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="917f7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="917f7-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="917f7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="917f7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganizations"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations
```
# <a name="c"></a>[<span data-ttu-id="917f7-135">C#</span><span class="sxs-lookup"><span data-stu-id="917f7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="917f7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="917f7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="917f7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="917f7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="917f7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="917f7-138">Response</span></span>
<span data-ttu-id="917f7-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="917f7-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
