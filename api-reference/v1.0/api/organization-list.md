---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe5d240a3ac8cf5ce722666080d764daeaa86589
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657786"
---
# <a name="list-organization"></a><span data-ttu-id="8abc9-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="8abc9-103">List organization</span></span>



<span data-ttu-id="8abc9-104">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="8abc9-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8abc9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8abc9-105">Permissions</span></span>
<span data-ttu-id="8abc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8abc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8abc9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8abc9-108">Permission type</span></span>      | <span data-ttu-id="8abc9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8abc9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8abc9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8abc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8abc9-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abc9-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="8abc9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8abc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8abc9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8abc9-113">Not supported.</span></span>    |
|<span data-ttu-id="8abc9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8abc9-114">Application</span></span> | <span data-ttu-id="8abc9-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abc9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="8abc9-116">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="8abc9-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="8abc9-117">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="8abc9-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="8abc9-118">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="8abc9-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="8abc9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8abc9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8abc9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8abc9-120">Optional query parameters</span></span>
<span data-ttu-id="8abc9-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8abc9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8abc9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8abc9-122">Request headers</span></span>
| <span data-ttu-id="8abc9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8abc9-123">Name</span></span>       | <span data-ttu-id="8abc9-124">Тип</span><span class="sxs-lookup"><span data-stu-id="8abc9-124">Type</span></span> | <span data-ttu-id="8abc9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8abc9-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8abc9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8abc9-126">Authorization</span></span>  | <span data-ttu-id="8abc9-127">string</span><span class="sxs-lookup"><span data-stu-id="8abc9-127">string</span></span>  | <span data-ttu-id="8abc9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8abc9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8abc9-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8abc9-130">Request body</span></span>
<span data-ttu-id="8abc9-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8abc9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8abc9-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="8abc9-132">Response</span></span>

<span data-ttu-id="8abc9-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8abc9-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8abc9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8abc9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8abc9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8abc9-135">Request</span></span>
<span data-ttu-id="8abc9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8abc9-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="8abc9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8abc9-137">Response</span></span>
<span data-ttu-id="8abc9-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8abc9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8abc9-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="8abc9-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8abc9-142">C#</span><span class="sxs-lookup"><span data-stu-id="8abc9-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8abc9-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="8abc9-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
