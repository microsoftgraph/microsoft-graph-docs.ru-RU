---
title: Получение организации
description: Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 54e5db4b3c8c0c279ef618e27911b8460a5669eb
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657303"
---
# <a name="get-organization"></a><span data-ttu-id="4780d-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="4780d-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4780d-104">Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="4780d-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="4780d-105">Так как ресурс **Организации** поддерживает [расширения](/graph/extensibility-overview), с помощью `GET` операции можно также получить настраиваемые свойства и данные расширения в экземпляре **Организации** .</span><span class="sxs-lookup"><span data-stu-id="4780d-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="4780d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4780d-106">Permissions</span></span>

<span data-ttu-id="4780d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4780d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4780d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4780d-109">Permission type</span></span> | <span data-ttu-id="4780d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4780d-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4780d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4780d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4780d-112">User. Read, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4780d-112">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="4780d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4780d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4780d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4780d-114">Not supported.</span></span> |
|<span data-ttu-id="4780d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4780d-115">Application</span></span> | <span data-ttu-id="4780d-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4780d-116">Directory.Read.All</span></span> |

> <span data-ttu-id="4780d-117">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="4780d-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="4780d-118">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="4780d-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="4780d-119">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="4780d-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="4780d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4780d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4780d-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4780d-121">Optional query parameters</span></span>

<span data-ttu-id="4780d-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4780d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4780d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4780d-123">Request headers</span></span>

| <span data-ttu-id="4780d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4780d-124">Name</span></span>       | <span data-ttu-id="4780d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4780d-125">Type</span></span> | <span data-ttu-id="4780d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4780d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4780d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4780d-127">Authorization</span></span>  | <span data-ttu-id="4780d-128">string</span><span class="sxs-lookup"><span data-stu-id="4780d-128">string</span></span>  | <span data-ttu-id="4780d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4780d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4780d-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4780d-131">Request body</span></span>

<span data-ttu-id="4780d-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4780d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4780d-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4780d-133">Response</span></span>

<span data-ttu-id="4780d-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4780d-134">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4780d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4780d-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4780d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4780d-136">Request</span></span>

<span data-ttu-id="4780d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4780d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="4780d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4780d-138">Response</span></span>

<span data-ttu-id="4780d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4780d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4780d-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4780d-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4780d-143">C#</span><span class="sxs-lookup"><span data-stu-id="4780d-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4780d-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="4780d-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="4780d-145">См. также</span><span class="sxs-lookup"><span data-stu-id="4780d-145">See also</span></span>

- [<span data-ttu-id="4780d-146">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="4780d-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4780d-147">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4780d-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
