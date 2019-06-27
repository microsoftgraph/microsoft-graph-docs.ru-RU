---
title: Получение организации
description: Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be18fda648cc2fc20e3e8a3697789d8de08a942c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266285"
---
# <a name="get-organization"></a><span data-ttu-id="0ccc4-103">Получение организации</span><span class="sxs-lookup"><span data-stu-id="0ccc4-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ccc4-104">Получение свойств и связей объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="0ccc4-105">Так как ресурс **Организации** поддерживает [расширения](/graph/extensibility-overview), с помощью `GET` операции можно также получить настраиваемые свойства и данные расширения в экземпляре **Организации** .</span><span class="sxs-lookup"><span data-stu-id="0ccc4-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ccc4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ccc4-106">Permissions</span></span>

<span data-ttu-id="0ccc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ccc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ccc4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ccc4-109">Permission type</span></span> | <span data-ttu-id="0ccc4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ccc4-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ccc4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ccc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ccc4-112">User. Read, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0ccc4-112">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="0ccc4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ccc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ccc4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-114">Not supported.</span></span> |
|<span data-ttu-id="0ccc4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ccc4-115">Application</span></span> | <span data-ttu-id="0ccc4-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ccc4-116">Directory.Read.All</span></span> |

> <span data-ttu-id="0ccc4-117">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="0ccc4-118">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="0ccc4-119">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="0ccc4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ccc4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ccc4-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ccc4-121">Optional query parameters</span></span>

<span data-ttu-id="0ccc4-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ccc4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ccc4-123">Request headers</span></span>

| <span data-ttu-id="0ccc4-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0ccc4-124">Name</span></span>       | <span data-ttu-id="0ccc4-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0ccc4-125">Type</span></span> | <span data-ttu-id="0ccc4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0ccc4-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0ccc4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ccc4-127">Authorization</span></span>  | <span data-ttu-id="0ccc4-128">string</span><span class="sxs-lookup"><span data-stu-id="0ccc4-128">string</span></span>  | <span data-ttu-id="0ccc4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ccc4-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ccc4-131">Request body</span></span>

<span data-ttu-id="0ccc4-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ccc4-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ccc4-133">Response</span></span>

<span data-ttu-id="0ccc4-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-134">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ccc4-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0ccc4-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ccc4-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ccc4-136">Request</span></span>

<span data-ttu-id="0ccc4-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="0ccc4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ccc4-138">Response</span></span>

<span data-ttu-id="0ccc4-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ccc4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0ccc4-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0ccc4-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0ccc4-143">C#</span><span class="sxs-lookup"><span data-stu-id="0ccc4-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ccc4-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ccc4-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0ccc4-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0ccc4-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_organization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="0ccc4-146">См. также</span><span class="sxs-lookup"><span data-stu-id="0ccc4-146">See also</span></span>

- [<span data-ttu-id="0ccc4-147">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="0ccc4-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0ccc4-148">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="0ccc4-148">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
