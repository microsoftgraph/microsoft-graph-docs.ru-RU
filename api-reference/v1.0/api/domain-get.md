---
title: Получение домена
description: Получение свойств и связей объекта домена.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1448336ac53503f4ee3e79b1c50a75e38d415298
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721238"
---
# <a name="get-domain"></a><span data-ttu-id="01fb9-103">Получение домена</span><span class="sxs-lookup"><span data-stu-id="01fb9-103">Get domain</span></span>

<span data-ttu-id="01fb9-104">Получение свойств и связей объекта домена.</span><span class="sxs-lookup"><span data-stu-id="01fb9-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="01fb9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01fb9-105">Permissions</span></span>

<span data-ttu-id="01fb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="01fb9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01fb9-108">Permission type</span></span>      | <span data-ttu-id="01fb9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01fb9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01fb9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01fb9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="01fb9-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="01fb9-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="01fb9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01fb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01fb9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01fb9-113">Not supported.</span></span>    |
|<span data-ttu-id="01fb9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01fb9-114">Application</span></span> | <span data-ttu-id="01fb9-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01fb9-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01fb9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01fb9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="01fb9-117">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="01fb9-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="01fb9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01fb9-118">Optional query parameters</span></span>

<span data-ttu-id="01fb9-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01fb9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01fb9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01fb9-120">Request headers</span></span>

| <span data-ttu-id="01fb9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="01fb9-121">Name</span></span>      |<span data-ttu-id="01fb9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="01fb9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01fb9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01fb9-123">Authorization</span></span>  | <span data-ttu-id="01fb9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01fb9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01fb9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01fb9-126">Content-Type</span></span>  | <span data-ttu-id="01fb9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="01fb9-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="01fb9-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01fb9-128">Request body</span></span>
<span data-ttu-id="01fb9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01fb9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01fb9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="01fb9-130">Response</span></span>

<span data-ttu-id="01fb9-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01fb9-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01fb9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="01fb9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01fb9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="01fb9-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="01fb9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="01fb9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="01fb9-135">C#</span><span class="sxs-lookup"><span data-stu-id="01fb9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01fb9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01fb9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01fb9-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="01fb9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="01fb9-138">Java</span><span class="sxs-lookup"><span data-stu-id="01fb9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="01fb9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="01fb9-139">Response</span></span>
<span data-ttu-id="01fb9-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01fb9-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
