---
title: Получение домена
description: Получение свойств и связей объекта домена.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7e5eaee09efa63c98ca3ee2ed6335863b73b1d80
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43179453"
---
# <a name="get-domain"></a><span data-ttu-id="2761d-103">Получение домена</span><span class="sxs-lookup"><span data-stu-id="2761d-103">Get domain</span></span>

<span data-ttu-id="2761d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2761d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2761d-105">Получение свойств и связей объекта домена.</span><span class="sxs-lookup"><span data-stu-id="2761d-105">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2761d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2761d-106">Permissions</span></span>

<span data-ttu-id="2761d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2761d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2761d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2761d-109">Permission type</span></span>      | <span data-ttu-id="2761d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2761d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2761d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2761d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2761d-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2761d-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="2761d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2761d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2761d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2761d-114">Not supported.</span></span>    |
|<span data-ttu-id="2761d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2761d-115">Application</span></span> | <span data-ttu-id="2761d-116">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2761d-116">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2761d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2761d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="2761d-118">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="2761d-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2761d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2761d-119">Optional query parameters</span></span>

<span data-ttu-id="2761d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2761d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2761d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2761d-121">Request headers</span></span>

| <span data-ttu-id="2761d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2761d-122">Name</span></span>      |<span data-ttu-id="2761d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2761d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2761d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2761d-124">Authorization</span></span>  | <span data-ttu-id="2761d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2761d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2761d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2761d-127">Content-Type</span></span>  | <span data-ttu-id="2761d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2761d-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2761d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2761d-129">Request body</span></span>
<span data-ttu-id="2761d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2761d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2761d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="2761d-131">Response</span></span>

<span data-ttu-id="2761d-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2761d-132">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2761d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2761d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2761d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2761d-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2761d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2761d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="2761d-136">C#</span><span class="sxs-lookup"><span data-stu-id="2761d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2761d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2761d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2761d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2761d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2761d-139">Java</span><span class="sxs-lookup"><span data-stu-id="2761d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2761d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2761d-140">Response</span></span>
<span data-ttu-id="2761d-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2761d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
