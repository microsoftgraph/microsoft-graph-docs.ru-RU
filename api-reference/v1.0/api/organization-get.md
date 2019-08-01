---
title: Получение организации
description: Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87b4284416e68b411bd772a86b9984f18848c6b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022686"
---
# <a name="get-organization"></a><span data-ttu-id="f49e0-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="f49e0-103">Get organization</span></span>

<span data-ttu-id="f49e0-104">Получение свойств и связей организации, прошедшей проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="f49e0-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="f49e0-105">Так как ресурс **organization** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете получить настраиваемые свойства и данные расширения в экземпляре **организации**.</span><span class="sxs-lookup"><span data-stu-id="f49e0-105">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="f49e0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f49e0-106">Permissions</span></span>

<span data-ttu-id="f49e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f49e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f49e0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f49e0-109">Permission type</span></span>      | <span data-ttu-id="f49e0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f49e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f49e0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f49e0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f49e0-112">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f49e0-112">User.Read, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="f49e0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f49e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f49e0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f49e0-114">Not supported.</span></span>    |
|<span data-ttu-id="f49e0-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f49e0-115">Application</span></span> | <span data-ttu-id="f49e0-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f49e0-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f49e0-117">**Примечание.** Приложения с разрешением User.Read могут считывать только такие свойства организации, как **id**, **displayName** и **verifiedDomains**.</span><span class="sxs-lookup"><span data-stu-id="f49e0-117">Note: Applications granted the User.Read permission are able to read only the id, displayName, and verifiedDomains properties of the organization.</span></span>  <span data-ttu-id="f49e0-118">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="f49e0-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="f49e0-119">Считать все свойства можно с помощью Organization.Read.All.</span><span class="sxs-lookup"><span data-stu-id="f49e0-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="f49e0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f49e0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f49e0-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f49e0-121">Optional query parameters</span></span>

<span data-ttu-id="f49e0-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f49e0-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f49e0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f49e0-123">Request headers</span></span>

| <span data-ttu-id="f49e0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f49e0-124">Name</span></span>       | <span data-ttu-id="f49e0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f49e0-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="f49e0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f49e0-126">Authorization</span></span>  | <span data-ttu-id="f49e0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f49e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f49e0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f49e0-129">Request body</span></span>

<span data-ttu-id="f49e0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f49e0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f49e0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f49e0-131">Response</span></span>

<span data-ttu-id="f49e0-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию из одного объекта [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f49e0-132">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f49e0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f49e0-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f49e0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f49e0-134">Request</span></span>

<span data-ttu-id="f49e0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f49e0-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f49e0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f49e0-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f49e0-137">C#</span><span class="sxs-lookup"><span data-stu-id="f49e0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f49e0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f49e0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f49e0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f49e0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f49e0-140">Java</span><span class="sxs-lookup"><span data-stu-id="f49e0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f49e0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f49e0-141">Response</span></span>

<span data-ttu-id="f49e0-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f49e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
