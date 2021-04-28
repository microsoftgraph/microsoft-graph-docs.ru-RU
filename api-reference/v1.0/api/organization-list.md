---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4d7fe6116fd33e7ad1ea46ff5d2179d9e8d23d81
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054534"
---
# <a name="list-organization"></a><span data-ttu-id="62b42-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="62b42-103">List organization</span></span>

<span data-ttu-id="62b42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62b42-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="62b42-105">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="62b42-105">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="62b42-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="62b42-106">Permissions</span></span>
<span data-ttu-id="62b42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62b42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62b42-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62b42-109">Permission type</span></span>      | <span data-ttu-id="62b42-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="62b42-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62b42-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62b42-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62b42-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b42-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="62b42-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62b42-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62b42-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62b42-114">Not supported.</span></span>    |
|<span data-ttu-id="62b42-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62b42-115">Application</span></span> | <span data-ttu-id="62b42-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b42-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="62b42-117">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="62b42-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="62b42-118">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="62b42-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="62b42-119">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="62b42-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="62b42-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62b42-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="62b42-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="62b42-121">Optional query parameters</span></span>
<span data-ttu-id="62b42-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="62b42-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="62b42-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62b42-123">Request headers</span></span>
| <span data-ttu-id="62b42-124">Имя</span><span class="sxs-lookup"><span data-stu-id="62b42-124">Name</span></span>       | <span data-ttu-id="62b42-125">Тип</span><span class="sxs-lookup"><span data-stu-id="62b42-125">Type</span></span> | <span data-ttu-id="62b42-126">Описание</span><span class="sxs-lookup"><span data-stu-id="62b42-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="62b42-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="62b42-127">Authorization</span></span>  | <span data-ttu-id="62b42-128">string</span><span class="sxs-lookup"><span data-stu-id="62b42-128">string</span></span>  | <span data-ttu-id="62b42-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62b42-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62b42-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62b42-131">Request body</span></span>
<span data-ttu-id="62b42-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62b42-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62b42-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="62b42-133">Response</span></span>

<span data-ttu-id="62b42-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62b42-134">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="62b42-135">Пример</span><span class="sxs-lookup"><span data-stu-id="62b42-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62b42-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="62b42-136">Request</span></span>
<span data-ttu-id="62b42-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62b42-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62b42-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="62b42-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="c"></a>[<span data-ttu-id="62b42-139">C#</span><span class="sxs-lookup"><span data-stu-id="62b42-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62b42-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62b42-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62b42-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62b42-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62b42-142">Java</span><span class="sxs-lookup"><span data-stu-id="62b42-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="62b42-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="62b42-143">Response</span></span>
<span data-ttu-id="62b42-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="62b42-144">Here is an example of the response.</span></span> <span data-ttu-id="62b42-145">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="62b42-145">Note: The response object shown here might be shortened for readability.</span></span>
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
          "assignedDateTime": "2017-07-29T02:16:28Z",
          "capabilityStatus": "Enabled",
          "service": "SharePoint",
          "servicePlanId": "5dbe027f-2339-4123-9542-606e4d348a72"
        }
      ],
      "businessPhones": [
        "8006427676"
      ],
      "city": "redmond",
      "country": null,
      "countryLetterCode": "US",
      "displayName": "Contoso"
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
