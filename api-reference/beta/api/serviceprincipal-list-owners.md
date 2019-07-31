---
title: 'СервицепринЦипалс: список владельцев'
description: Получение списка владельцев servicePrincipal.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a221699069f06c8825ac29d65c5730f3f4a56df1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991340"
---
# <a name="serviceprincipals-list-owners"></a><span data-ttu-id="aae52-103">СервицепринЦипалс: список владельцев</span><span class="sxs-lookup"><span data-stu-id="aae52-103">servicePrincipals: List owners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aae52-104">Получение списка владельцев servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="aae52-104">Retrieve a list of owners of the servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="aae52-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aae52-105">Permissions</span></span>
<span data-ttu-id="aae52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aae52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aae52-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aae52-108">Permission type</span></span>      | <span data-ttu-id="aae52-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aae52-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aae52-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aae52-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aae52-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aae52-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aae52-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aae52-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aae52-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aae52-113">Not supported.</span></span>    |
|<span data-ttu-id="aae52-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aae52-114">Application</span></span> | <span data-ttu-id="aae52-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae52-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aae52-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aae52-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aae52-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aae52-117">Optional query parameters</span></span>
<span data-ttu-id="aae52-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aae52-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aae52-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aae52-119">Request headers</span></span>
| <span data-ttu-id="aae52-120">Имя</span><span class="sxs-lookup"><span data-stu-id="aae52-120">Name</span></span>       | <span data-ttu-id="aae52-121">Тип</span><span class="sxs-lookup"><span data-stu-id="aae52-121">Type</span></span> | <span data-ttu-id="aae52-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aae52-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aae52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aae52-123">Authorization</span></span>  | <span data-ttu-id="aae52-124">string</span><span class="sxs-lookup"><span data-stu-id="aae52-124">string</span></span>  | <span data-ttu-id="aae52-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aae52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aae52-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aae52-127">Request body</span></span>
<span data-ttu-id="aae52-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aae52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aae52-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aae52-129">Response</span></span>

<span data-ttu-id="aae52-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aae52-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aae52-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aae52-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aae52-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aae52-132">Request</span></span>
<span data-ttu-id="aae52-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aae52-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="aae52-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="aae52-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/owners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aae52-135">C#</span><span class="sxs-lookup"><span data-stu-id="aae52-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aae52-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="aae52-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aae52-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="aae52-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="aae52-138">Java</span><span class="sxs-lookup"><span data-stu-id="aae52-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aae52-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="aae52-139">Response</span></span>
<span data-ttu-id="aae52-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aae52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
