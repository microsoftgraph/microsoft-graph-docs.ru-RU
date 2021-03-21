---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fcfca5ed7d51949dc5bd479ec98491bac6ff4eee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955868"
---
# <a name="list-organization"></a><span data-ttu-id="c05fa-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="c05fa-103">List organization</span></span>

<span data-ttu-id="c05fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c05fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c05fa-105">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="c05fa-105">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c05fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c05fa-106">Permissions</span></span>
<span data-ttu-id="c05fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c05fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c05fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c05fa-109">Permission type</span></span>      | <span data-ttu-id="c05fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c05fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c05fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c05fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c05fa-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c05fa-112">Not supported.</span></span>    |
|<span data-ttu-id="c05fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c05fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c05fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c05fa-114">Not supported.</span></span>    |
|<span data-ttu-id="c05fa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c05fa-115">Application</span></span> | <span data-ttu-id="c05fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c05fa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c05fa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c05fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c05fa-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c05fa-118">Optional query parameters</span></span>
<span data-ttu-id="c05fa-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c05fa-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c05fa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c05fa-120">Request headers</span></span>
| <span data-ttu-id="c05fa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c05fa-121">Name</span></span>       | <span data-ttu-id="c05fa-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c05fa-122">Type</span></span> | <span data-ttu-id="c05fa-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c05fa-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c05fa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c05fa-124">Authorization</span></span>  | <span data-ttu-id="c05fa-125">string</span><span class="sxs-lookup"><span data-stu-id="c05fa-125">string</span></span>  | <span data-ttu-id="c05fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c05fa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c05fa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c05fa-128">Request body</span></span>
<span data-ttu-id="c05fa-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c05fa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c05fa-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c05fa-130">Response</span></span>

<span data-ttu-id="c05fa-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c05fa-131">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c05fa-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c05fa-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c05fa-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c05fa-133">Request</span></span>
<span data-ttu-id="c05fa-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c05fa-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c05fa-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c05fa-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="c"></a>[<span data-ttu-id="c05fa-136">C#</span><span class="sxs-lookup"><span data-stu-id="c05fa-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c05fa-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c05fa-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c05fa-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c05fa-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c05fa-139">Java</span><span class="sxs-lookup"><span data-stu-id="c05fa-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c05fa-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c05fa-140">Response</span></span>
<span data-ttu-id="c05fa-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c05fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
