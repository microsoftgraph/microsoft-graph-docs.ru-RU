---
title: Получение организации
description: Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 124f4a05f30196b622b62ecd82ea15a892e3682b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448335"
---
# <a name="get-organization"></a><span data-ttu-id="c09f9-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="c09f9-103">Get organization</span></span>

<span data-ttu-id="c09f9-104">Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="c09f9-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c09f9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c09f9-105">Permissions</span></span>

<span data-ttu-id="c09f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c09f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c09f9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c09f9-108">Permission type</span></span>      | <span data-ttu-id="c09f9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c09f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c09f9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c09f9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c09f9-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c09f9-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="c09f9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c09f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c09f9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c09f9-113">Not supported.</span></span>    |
|<span data-ttu-id="c09f9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c09f9-114">Application</span></span> | <span data-ttu-id="c09f9-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c09f9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="c09f9-116">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="c09f9-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="c09f9-117">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="c09f9-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="c09f9-118">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="c09f9-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="c09f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c09f9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c09f9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c09f9-120">Optional query parameters</span></span>

<span data-ttu-id="c09f9-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c09f9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c09f9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c09f9-122">Request headers</span></span>

| <span data-ttu-id="c09f9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c09f9-123">Name</span></span>       | <span data-ttu-id="c09f9-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c09f9-124">Type</span></span> | <span data-ttu-id="c09f9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c09f9-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c09f9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c09f9-126">Authorization</span></span>  | <span data-ttu-id="c09f9-127">string</span><span class="sxs-lookup"><span data-stu-id="c09f9-127">string</span></span>  | <span data-ttu-id="c09f9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c09f9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c09f9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c09f9-130">Request body</span></span>

<span data-ttu-id="c09f9-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c09f9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c09f9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c09f9-132">Response</span></span>

<span data-ttu-id="c09f9-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию из одного объекта [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c09f9-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c09f9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c09f9-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c09f9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c09f9-135">Request</span></span>

<span data-ttu-id="c09f9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c09f9-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c09f9-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c09f9-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c09f9-138">C#</span><span class="sxs-lookup"><span data-stu-id="c09f9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c09f9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c09f9-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c09f9-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c09f9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c09f9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c09f9-141">Response</span></span>

<span data-ttu-id="c09f9-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c09f9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
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
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
