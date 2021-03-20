---
title: Получение организации
description: Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.
localization_priority: Priority
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 836f7b0531c0700d6f135448f0c27ba1c8aa6abd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949640"
---
# <a name="get-organization"></a><span data-ttu-id="30df3-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="30df3-103">Get organization</span></span>

<span data-ttu-id="30df3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30df3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30df3-105">Получение свойств и связей организации, прошедшей проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="30df3-105">Get the properties and relationships of the currently authenticated organization.</span></span>

<span data-ttu-id="30df3-106">Так как ресурс **organization** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` вы можете получить настраиваемые свойства и данные расширения в экземпляре **организации**.</span><span class="sxs-lookup"><span data-stu-id="30df3-106">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="30df3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30df3-107">Permissions</span></span>

<span data-ttu-id="30df3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30df3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30df3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30df3-110">Permission type</span></span>      | <span data-ttu-id="30df3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30df3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30df3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30df3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="30df3-113">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30df3-113">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="30df3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30df3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30df3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30df3-115">Not supported.</span></span>    |
|<span data-ttu-id="30df3-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="30df3-116">Application</span></span> | <span data-ttu-id="30df3-117">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30df3-117">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="30df3-118">**Примечание.** Приложения с разрешением User.Read могут считывать только такие свойства организации, как **id**, **displayName** и **verifiedDomains**.</span><span class="sxs-lookup"><span data-stu-id="30df3-118">**Note**: Applications granted the User.Read permission are able to read only the **id**, **displayName**, and **verifiedDomains** properties of the organization.</span></span>  <span data-ttu-id="30df3-119">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="30df3-119">All other properties will return with `null` values.</span></span> <span data-ttu-id="30df3-120">Считать все свойства можно с помощью Organization.Read.All.</span><span class="sxs-lookup"><span data-stu-id="30df3-120">To read all properties, use Organization.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="30df3-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30df3-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30df3-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30df3-122">Optional query parameters</span></span>

<span data-ttu-id="30df3-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30df3-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30df3-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30df3-124">Request headers</span></span>

| <span data-ttu-id="30df3-125">Имя</span><span class="sxs-lookup"><span data-stu-id="30df3-125">Name</span></span>       | <span data-ttu-id="30df3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="30df3-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="30df3-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30df3-127">Authorization</span></span>  | <span data-ttu-id="30df3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30df3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30df3-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30df3-130">Request body</span></span>

<span data-ttu-id="30df3-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30df3-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30df3-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="30df3-132">Response</span></span>

<span data-ttu-id="30df3-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию из одного объекта [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30df3-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30df3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="30df3-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="30df3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="30df3-135">Request</span></span>

<span data-ttu-id="30df3-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30df3-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="30df3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="30df3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="c"></a>[<span data-ttu-id="30df3-138">C#</span><span class="sxs-lookup"><span data-stu-id="30df3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30df3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30df3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30df3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30df3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30df3-141">Java</span><span class="sxs-lookup"><span data-stu-id="30df3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="30df3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="30df3-142">Response</span></span>

<span data-ttu-id="30df3-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30df3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
