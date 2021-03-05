---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f11ed888ad14334584a8f2e6aea9bb821f86438f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441734"
---
# <a name="list-organization"></a><span data-ttu-id="0af9c-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="0af9c-103">List organization</span></span>

<span data-ttu-id="0af9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0af9c-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="0af9c-105">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="0af9c-105">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0af9c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0af9c-106">Permissions</span></span>
<span data-ttu-id="0af9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0af9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af9c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0af9c-109">Permission type</span></span>      | <span data-ttu-id="0af9c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0af9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0af9c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0af9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0af9c-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af9c-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="0af9c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0af9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0af9c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0af9c-114">Not supported.</span></span>    |
|<span data-ttu-id="0af9c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0af9c-115">Application</span></span> | <span data-ttu-id="0af9c-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af9c-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="0af9c-117">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="0af9c-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="0af9c-118">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="0af9c-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="0af9c-119">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="0af9c-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="0af9c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0af9c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0af9c-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0af9c-121">Optional query parameters</span></span>
<span data-ttu-id="0af9c-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0af9c-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0af9c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0af9c-123">Request headers</span></span>
| <span data-ttu-id="0af9c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0af9c-124">Name</span></span>       | <span data-ttu-id="0af9c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0af9c-125">Type</span></span> | <span data-ttu-id="0af9c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0af9c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0af9c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af9c-127">Authorization</span></span>  | <span data-ttu-id="0af9c-128">string</span><span class="sxs-lookup"><span data-stu-id="0af9c-128">string</span></span>  | <span data-ttu-id="0af9c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0af9c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0af9c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0af9c-131">Request body</span></span>
<span data-ttu-id="0af9c-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0af9c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0af9c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0af9c-133">Response</span></span>

<span data-ttu-id="0af9c-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0af9c-134">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0af9c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0af9c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0af9c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0af9c-136">Request</span></span>
<span data-ttu-id="0af9c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0af9c-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0af9c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0af9c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="c"></a>[<span data-ttu-id="0af9c-139">C#</span><span class="sxs-lookup"><span data-stu-id="0af9c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0af9c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0af9c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0af9c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0af9c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0af9c-142">Java</span><span class="sxs-lookup"><span data-stu-id="0af9c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0af9c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0af9c-143">Response</span></span>
<span data-ttu-id="0af9c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0af9c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
